<script>
export default {
    name: 'AppHeader'
}
</script>
<template>
    <header>
        <div class="container">
            <div class="row">
                <div>
                    <img src="/dc-logo.png" alt="">
                </div>
                <ul>
                    <li><a href="">CHARACTERS</a></li>
                    <li><a href="">COMICS</a></li>
                    <li><a href="">MOVIES</a></li>
                    <li><a href="">TV</a></li>
                    <li><a href="">GAMES</a></li>
                    <li><a href="">COLLECTIBLES</a></li>
                    <li><a href="">VIDEOS</a></li>
                    <li><a href="">FANS</a></li>
                    <li><a href="">NEWS</a></li>
                    <li><a href="">SHOP</a></li>
                </ul>
            </div>
        </div>
    </header>
</template>
<style scoped>
.row {
    padding: 0.5rem;
}

ul {
    display: flex;
    list-style: none;

    li {
        padding: 0.5rem;
        margin-bottom: -2rem;
    }

    li::after {
        display: block;
        content: "";
        border-bottom: solid 5px var(--bg-text-lightblue);
        transition: all 0s ease-in-out 0s;
        transform: scaleX(0);
        padding-bottom: 2rem;

    }

    li:hover{
        
        a {
            color: var(--bg-text-lightblue);
        }
        
    }

    li:hover::after {
        transform: scaleX(1);
    }

    a {
        text-decoration: none;
        color: var(--nav-text-grey);
        font-weight: 700;
    }
    
}
</style>