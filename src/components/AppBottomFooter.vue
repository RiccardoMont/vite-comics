<script>

export default {
    name: 'AppBottomFooter',
    data() {
        return {
            loghi: [
                {
                    name: 'facebook',
                    img: '/footer-facebook.png'
                },
                {
                    name: 'twitter',
                    img: '/footer-twitter.png'
                },
                {
                    name: 'youtube',
                    img: '/footer-youtube.png'
                },
                {
                    name: 'pinteres',
                    img: '/footer-pinterest.png'
                },
                {
                    name: 'periscope',
                    img: '/footer-periscope.png'
                }
            ]
        }
    },
}
</script>
<template>
<div class="bottomFooter">
        <div class="container">
            <div class="row">
                <button>SIGN-UP NOW!</button>
                <div class="socials">
                    <h3>FOLLOW US</h3>
                    <a href="" v-for="logo in loghi"><img :src="logo.img" :alt="logo.text"></a>
                </div>
            </div>
        </div>
    </div>

</template>
<style>


.bottomFooter {
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
</style>