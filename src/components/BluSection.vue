<script>
import { assert } from '@vue/compiler-core';

export default {
    data() {
        return {
            items: [
                {
                    img: "../assets/img/buy-comics-digital-comics.png",
                    text: "DIGITAL COMICS",
                    url: "#"
                }
            ]
        }
    }
}
</script>

<template>
    <section class="container">
        <ul>
            <li v-for="item in items">
                <img :src="item.img" alt="">
                <a :href="item.url"> {{ item.text }} </a>
            </li>
        </ul>
    </section>
</template>

<style lang="scss">
@use '../temp/partials/mixins.scss' as *;
@use '../temp/partials/variables.scss' as *;
</style>