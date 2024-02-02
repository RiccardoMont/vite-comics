<script>
export default {
    name: 'AppMain',

}
</script>
<template>
    <div class="content">
        <div class="container">
            <h2>Content goes here</h2>
        </div>

    </div>
    <div class="comicsLocations">
        <div class="container">
            <div class="row">
                <a class="singleIcon" href="#">
                    <img class="resizeIcon" src="/buy-comics-digital-comics.png" alt="">
                    <span>DIGITAL COMICS</span>
                </a>
                <a class="singleIcon" href="#">
                    <img class="resizeIcon" src="/buy-comics-merchandise.png" alt="">
                    <span>DC MERCHANDISE</span>
                </a>
                <a class="singleIcon" href="#">
                    <img class="resizeIcon" src="/buy-comics-subscriptions.png" alt="">
                    <span>SUBSCRIPTION</span>
                </a>
                <a class="singleIcon" href="#">
                    <img class="resizeIcon" src="/buy-comics-shop-locator.png" alt="">
                    <span>COMIC SHOP LOCATOR</span>
                </a>
                <a class="singleIcon" href="#">
                    <img class="resizeIcon" src="/buy-dc-power-visa.svg" alt="">
                    <span class="alfa">DC POWER VISA</span>
                </a>
            </div>
        </div>
    </div>
</template>
<style scoped>
.content {
    height: 100px;
    background-color: var(--bg-main-black);

    & h2 {
        color: var(--main-footer-titles-white);
    }
}

.comicsLocations {
    height: 18vh;
    width: 100vw;
    background-color: var(--bg-text-lightblue);
    display: flex;
    align-items: center;
    position: relative;
    z-index: 2;


}

.row {
    justify-content: space-evenly;
    flex-wrap: nowrap;
}

.singleIcon {
    display: flex;
    align-items: center;
    justify-content: start;
    text-decoration: none;

    & span {
        color: var(--main-footer-titles-white);
        font-size: 15px;
        white-space: nowrap;
    }
}

.resizeIcon {
    max-width: 65px;
    max-height: 65px;
}
</style>