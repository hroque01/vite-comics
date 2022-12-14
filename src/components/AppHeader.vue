<script>
export default {
    data() {
        name: 'AppHeader'
        navMenu: [
            {
                navigation: "CHARACTERS"
            },
            {
                navigation: "COMICS"
            },
            {
                navigation: "MOVIES"
            },
            {
                navigation: "TV"
            },
            {
                navigation: "GAMES"
            },
            {
                navigation: "CHARACTERS"
            },
            {
                navigation: "COLLECTIBLES"
            },
            {
                navigation: "VIDEOS"
            },
            {
                navigation: "FANS"
            },
            {
                navigation: "NEWS"
            },
            {
                navigation: "SHOP"
            }
        ]
    }
}
</script>

<template>

    <header>
        <a href="#">
            <img src="/dc-logo-bg.png" alt="">
        </a>
    </header>

</template>

<style lang="scss" scoped>
header {
    text-align: center;
}
</style>