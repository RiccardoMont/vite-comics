<script>

export default {
    name: 'AppTopFooter'
}
</script>
<template>
<div class="categories">
        <div class="container">
            <div class="row">
                <div class="links">
                    <div class="col-4">
                        <h5>DC COMICS</h5>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                        <h5>SHOP</h5>
                        <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                    <div class="col-4">
                        <h5>DC</h5>
                        <ul>
                            <li><a href="#">Terms of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="#">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                        </ul>
                    </div>
                    <div class="col-4">
                        <h5>SITES</h5>
                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
.row {
    flex-wrap: nowrap;
}


.categories {
    background-image:url('/dc-logo-bg.png'), url('/footer-bg.jpg');
    background-repeat: no-repeat, no-repeat;
    background-size: 500px, cover;
    background-position-x: 80%;
    background-position-y: 40%;
    width: 100vw;


    & ul {
        list-style: none;
    }
}



.links {
    display: flex;
    margin-left: -1rem;
    padding: 2rem 0;


    & li {
        line-height: 1;

    }

    & h5 {
        color: var(--main-footer-titles-white);
        padding-bottom: 5px;
        padding-top: 10px;
    }

    & a {
        text-decoration: none;
        color: var(--footer-text-grey);
        font-size: 10px;
    }


    & .col-4 {
        width: calc((100%/12)*4);
        padding-left: 10px;
        padding-right: 1rem;
    }
}
</style>