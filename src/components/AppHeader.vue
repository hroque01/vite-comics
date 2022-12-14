<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: '#',
                    current: false,
                },
                {
                    text: "COMICS",
                    url: '#',
                    current: true,
                },
                {
                    text: "MOVIES",
                    url: '#',
                    current: false,
                },
                {
                    text: "TV",
                    url: '#',
                    current: false,
                },
                {
                    text: "GAMES",
                    url: '#',
                    current: false,
                },
                {
                    text: "COLLECTIBLES",
                    url: '#',
                    current: false,
                },
                {
                    text: "VIDEOS",
                    url: '#',
                    current: false,
                },
                {
                    text: "FANS",
                    url: '#',
                    current: false,
                },
                {
                    text: "NEWS",
                    url: '#',
                    current: false,
                },
                {
                    text: "SHOP",
                    url: '#',
                    current: false,
                }
            ]
        }
    }
}
</script>

<template>

    <header>
        <a href="#">
            <img src="/dc-logo.png" alt="">
        </a>
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :class="{ active: link.current }" :href="link.url">
                        {{ link.text }}
                    </a>
                </li>
            </ul>
        </nav>
    </header>

</template>

<style lang="scss" scoped>
@use '../temp/partials/mixins.scss' as *;
@use '../temp/partials/variables.scss' as *;

header {
    text-align: center;
}

ul {
    list-style: none;
    margin: 2.5 1rem 4rem;
    @include center();

    li a {
        display: inline-block;
        padding: 1rem;
        text-decoration: none;
        font-weight: 600;

        &.active,
        &:hover {
            background: lighten($color: $secondary, $amount: 70%);
            color: $secondary;
        }
    }
}
</style>