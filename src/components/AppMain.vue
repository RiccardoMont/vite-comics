<script>
import AppJumbotron from './AppJumbotron.vue';
import AppComicsList from './AppComicsList.vue';
import AppComicsLocation from './AppComicsLocation.vue';

export default {
    name: 'AppMain',
    
    components: {
        AppJumbotron,
        AppComicsList,
        AppComicsLocation
    }
}
</script>
<template>
<AppJumbotron></AppJumbotron>
<AppComicsList></AppComicsList>
<AppComicsLocation></AppComicsLocation>
    
    
</template>
<style scoped>

</style>