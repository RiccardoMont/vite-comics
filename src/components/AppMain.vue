<script>

export default {
    name: 'AppMain',
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
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg/revision/latest?cb=20080809201655",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg/revision/latest/scale-to-width-down/1200?cb=20130627211607",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg/revision/latest?cb=20200929145132",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg/revision/latest?cb=20200929124651",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg/revision/latest?cb=20201123054610",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg/revision/latest?cb=20201124094800",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg/revision/latest?cb=20160303223223",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    }
}
</script>
<template>
    <div class="content">
        <div class="container">
            <div class="row">
                <div class="comicCard" v-for="comic in comics">
                    <img class="resizeComic" :src=comic.thumb alt="">
                    <h4>{{ comic.series }}</h4>
                </div>
            </div>
            <div class="loadMore">
                <button>LOAD MORE</button>
            </div>

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
    background-color: var(--bg-main-black);

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
    margin-left: -1rem;
    margin-right: -1rem;
    padding: 1rem;


    & h4 {
        font-weight: 400;
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
    flex-wrap: wrap;
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

.resizeComic {
    height: 150px;
    width: 150px;
    max-width: 150px;
    max-height: 150px;
}
</style>