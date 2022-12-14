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
                    current: false,
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
                <li>
                    <a class="active" href="#">
                        CHARACTERS
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
        transition: background 0.3s;

        &.active,
        &:hover {
            background-color: lighten($color: blue, $amount: 70%);
        }
    }
}
</style>