<script>
export default {
    name: 'AppComicsLocations',
    data() {
        return{
            icons: [
                {
                    text: 'DIGITAL COMICS',
                    img: '/buy-comics-digital-comics.png'
                },
                {
                    text: 'DC MERCHANDISE',
                    img: '/buy-comics-merchandise.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    img: '/buy-comics-subscriptions.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    img: '/buy-comics-shop-locator.png'
                },
                {
                    text: 'DC POWER VISA',
                    img: '/buy-dc-power-visa.svg'
                }
            ]
        }
    }
}
</script>
<template>
    <div class="comicsLocations">
        <div class="container">
            <div class="row">
                <div class="singleIcon" v-for="icon in icons">
                    <img class="resizeIcon" :src="icon.img" alt="">
                    <span>{{ icon.text }}</span>
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
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
    align-items: center;
    flex-wrap: wrap;
}


.singleIcon {
    display: flex;
    align-items: center;
    justify-content: start;
    text-decoration: none;
    cursor: pointer;

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