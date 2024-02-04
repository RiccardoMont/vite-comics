<script>
import AppCardComic from './AppCardComic.vue';
export default{
    name: 'AppComicsList',
    data() {
        return {
            comics: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    },
    components: {
        AppCardComic
    }
}
</script>
<template>
    <div class="content">
        <div class="container">
            <h3>Current Series</h3>
            <div class="row">
                <div class="comicCard" v-for="(comic, index) in comics" :key="index + ' ' + comic.series">
                    <AppCardComic :series="comic.series" :thumb="comic.thumb" ></AppCardComic>
                </div>
            </div>
            <div class="loadMore">
                <button>LOAD MORE</button>
            </div>

        </div>

    </div>
</template>
<style scoped>
.content {
    background-color: var(--bg-main-black);

    & h3 {
        display: inline-block;
        padding: 1rem;
        background-color: var(--bg-text-lightblue);
        color: var(--main-footer-titles-white);
        margin-top: -20px;
    }

    & h2 {
        color: var(--main-footer-titles-white);
    }

    & .row {
        align-items: start;
        gap: 1rem;
    }

    & .loadMore {
        display: flex;
        justify-content: center;
    }

    & button {
        background-color: var(--bg-text-lightblue);
        margin: 2rem;
        padding: 1rem;
        font-size: 16px;
        font-weight: 700;
        color: var(--main-footer-titles-white);
        border: 1px solid var(--bg-text-lightblue);
        cursor: pointer;
    }

    & button:hover {

        background-color: rgb(8, 42, 122);
    }
}

.comicCard {
    width: calc((100%/12)*2);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 0 -1rem;
    padding: 1rem;

}


</style>