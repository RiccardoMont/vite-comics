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
                <div class="imgDiv">
                    <img class="resizeLogo" src="/dc-logo-bg.png" alt="">
                </div>

                <!--<div class="mark">
                    <img class="resizeLogo" src="/dc-logo-bg.png" alt="">
                </div>-->

            </div>
        </div>
    </div>
    <div class="signSocial">
        <div class="container">
            <div class="row">
                <button>SIGN-UP NOW!</button>
                <div class="socials">
                    <h3>FOLLOW US</h3>
                    <a href=""><img src="/footer-facebook.png" alt=""></a>
                    <a href=""><img src="/footer-twitter.png" alt=""></a>
                    <a href=""><img src="/footer-youtube.png" alt=""></a>
                    <a href=""><img src="/footer-pinterest.png" alt=""></a>
                    <a href=""><img src="/footer-periscope.png" alt=""></a>
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
    background-image: url('/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: 100%;
    width: 100vw;


    & ul {
        list-style: none;
    }
}



.links {
    display: flex;
    margin-left: -1rem;


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

.imgDiv{
    position: relative;
    margin-bottom: -74px;
    margin-top: -80px;
    display: flex;
    justify-content: end;
}

.signSocial {
    background-color: var(--bg-socials);
    height: 10vh;
    min-height: 60px;
    width: 100%;
    display: flex;
    align-items: center;
    position: relative;
    z-index: 2;

    & .row {

        margin-left: -10px;
    }

    & button {
        background-color: var(--bg-socials);
        color: var(--main-footer-titles-white);
        padding: 10px;
        border: 2px solid var(--bg-text-lightblue);
        font-weight: 600;
        min-width: 100px;
        cursor: pointer;
    }

    .socials {
        display: flex;
        align-items: center;
        gap: 10px;
        min-width: 120px;

        & h3 {
            color: var(--bg-text-lightblue);
        }

    }
}


.resizeLogo {
    width: 85%;
}
</style>