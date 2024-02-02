<script>
export default {
    name: 'AppFooter',
}
</script>
<template>
    <div class="categories">
        <div class="container">
            <div class="row">
                <div class="links">
                    <div class="col-4">
                        <h4>DC COMICS</h4>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                        <h4>SHOP</h4>
                        <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                    <div class="col-4">
                        <h4>DC</h4>
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
                        <h4>SITES</h4>
                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>

                </div>
                <div class="mark">
                    <img class="resizeLogo" src="/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
    </div>
    <div class="socials">
    </div>
</template>
<style scoped>
.categories {
    background-image: url('/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: 100%;
    width: 100vw;
    position: fixed;
    bottom: 0;
    left: 0;
    z-index: -1;


    & ul {
        list-style: none;
    }
}

.links {
    display: flex;
    margin-left: -1rem;

    & ul {
        padding-bottom: 5px;
    }

    & h4 {
        color: var(--main-footer-titles-white);
        padding-bottom: 5px;
    }

    & a {
        text-decoration: none;
        color: var(--footer-text-grey);
        font-size: 12px;
    }


    & .col-4 {
        width: calc((100%/12)*4);
        padding-left: 1rem;
        padding-right: 1rem;
    }
}

.socials {
    height: 10vh;
    width: 100vw;
    background-color: var(--bg-socials);
    position: absolute;
    bottom: 0px;
    left: 0px;
    z-index: 5;
}

.resizeLogo {
    height: 60vh;
}
</style>