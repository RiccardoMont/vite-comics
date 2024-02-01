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
                <div class="singleIcon">
                    <img class="resizeIcon" src="/buy-comics-digital-comics.png" alt="">
                    <span>DIGITAL COMICS</span>
                </div>
                <div class="singleIcon">
                    <img class="resizeIcon" src="/buy-comics-merchandise.png" alt="">
                    <span>DC MERCHANDISE</span>
                </div>
                <div class="singleIcon">
                    <img class="resizeIcon" src="/buy-comics-subscriptions.png" alt="">
                    <span>SUBSCRIPTION</span>
                </div>

                <div class="singleIcon">
                    <img class="resizeIcon" src="/buy-comics-shop-locator.png" alt="">
                    <span>COMIC SHOP LOCATOR</span>
                </div>
                <div class="singleIcon">
                    <img class="resizeIcon" src="/buy-dc-power-visa.svg" alt="">
                    <span class="alfa">DC POWER VISA</span>
                </div>


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
    height: 150px;
    background-color: var(--bg-text-lightblue);
    display: flex;
    align-items: center;
}

.row {
    justify-content: space-evenly;
    flex-wrap: nowrap;
}

.singleIcon {
    display: flex;
    align-items: center;
    justify-content: start;

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