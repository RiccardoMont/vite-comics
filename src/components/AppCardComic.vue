<script>
export default {
    name: 'AppCardComic',
    props: {
        thumb: String,
        series: String
    }
}
</script>
<template>
    <div class="maskComic">
        <img class="resizeComic" :src="thumb" alt="">
    </div>
    <h4>{{ series }}</h4>
</template>
<style scoped>
.maskComic {
    overflow: hidden;
    width: 150px;
    height: 200px;
    max-width: 150px;
    max-height: 200px;


}

h4 {
    font-weight: 400;
    color: var(--main-footer-titles-white);
}

.resizeComic {
    height: 200px;

}
</style>