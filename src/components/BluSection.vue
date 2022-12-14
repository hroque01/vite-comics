<script>
export default {
    data() {
        return {
            items: [
                {
                    img: "/img/buy-comics-digital-comics.png",
                    text: "DIGITAL COMICS",
                    url: "#"
                },
                {
                    img: "/img/buy-comics-merchandise.png",
                    text: "DC MERCHANDISE",
                    url: "#"
                },
                {
                    img: "/img/buy-comics-subscriptions.png",
                    text: "SUBSCRIPTION",
                    url: "#"
                },
                {
                    img: "/img/buy-comics-shop-locator.png",
                    text: "COMIC CHOP LOCATOR",
                    url: "#"
                },
                {
                    img: "/img/buy-dc-power-visa.svg",
                    text: "DC POWER VISA",
                    url: "#"
                }

            ]
        }
    }
}
</script>

<template>
    <section class="merch">
        <ul class="container">
            <li class="merch-list" v-for="item in items">
                <img class="merch-img" :src="item.img" alt="">
                <a :href="item.url"> {{ item.text }} </a>
            </li>
        </ul>
    </section>
</template>

<style lang="scss">
@use '../temp/partials/mixins.scss' as *;
@use '../temp/partials/variables.scss' as *;

.merch {
    padding: 20px;
    background-color: #0282f9;

    ul {
        display: flex;
        justify-content: space-between;
        list-style: none;
        margin: 2.5 1rem 4rem;
    }

    .merch-list {

        display: flex;
        align-items: center;
        margin: 20px;

        .merch-img {

            width: 40px;

        }

        a {
            padding: 10px;
            color: white;
        }
    }
}
</style>