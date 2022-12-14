<script>
export default {
    data() {
        return {
            comics: [
                "Characters",
                "Comics",
                "Movies",
                "TV",
                "Games",
                "Videos",
                "News"
            ],
            shops: [
                "Shop DC",
                "Shop DC Collectibles"
            ],
            dc: [
                "Terme of Use",
                "Privacy Policy (New)",
                "Ad Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshop",
                "CPCS Certificates",
                "Ratings",
                "Shop Help",
                "Contact us"
            ],
            sites: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa"
            ]
        }
    }
}
</script>

<template>
    <section class="links">
        <div class="container links">

            <div>
                <h1>DC COMICS</h1>
                <div v-for="comic in comics">
                    <a href="#">{{ comic }}</a>
                </div>
                <h1>SHOP</h1>
                <div v-for="shop in shops">
                    <a href="3">{{ shop }}</a>
                </div>
            </div>
            <div>
                <h1>DC</h1>
                <div v-for="information in dc">
                    <a href="#">{{ information }}</a>
                </div>
            </div>
            <div>
                <h1>SITES</h1>
                <div v-for="site in sites">
                    <a href="#">{{ site }}</a>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../temp/partials/mixins.scss' as *;
@use '../temp/partials/variables.scss' as *;

.links {
    display: flex;
}
</style>