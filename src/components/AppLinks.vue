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
    <section>
        <div class="links">
            <div class="container">
                <div class="title-links">
                    <h1>DC COMICS</h1>
                    <div class="arrays-link" v-for="comic in comics">
                        <a href="#">{{ comic }}</a>
                    </div>
                    <h1>SHOP</h1>
                    <div class="arrays-link" v-for="shop in shops">
                        <a href="3">{{ shop }}</a>
                    </div>
                </div>

                <div class="title-links">
                    <h1>DC</h1>
                    <div class="arrays-link" v-for="information in dc">
                        <a href="#">{{ information }}</a>
                    </div>
                </div>

                <div class="title-links">
                    <h1>SITES</h1>
                    <div class="arrays-link" v-for="site in sites">
                        <a href="#">{{ site }}</a>
                    </div>
                </div>

                <div class="img-bg">
                    <img src="/dc-logo-bg.png" alt="">
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
    margin: 0;
    background-image: url(img/footer-bg.jpg);
    background-size: cover;
    position: relative;
    overflow: hidden;

    .container {
        display: flex;
        margin: 0;
        padding: 0 10px;

    }

    .link-parts {
        display: flex;
    }

    .title-links {
        display: flex;
        flex-direction: column;
        margin-left: 50px;
        padding-bottom: 50px;
        font-size: 16px;

        h1 {
            padding-top: 30px;
            padding-bottom: 10px;
            color: white;
        }

        .arrays-link {
            display: flex;
            padding-top: 5px;

            a {
                height: 25px;
                color: #676d69;
            }
        }
    }
}

.img-bg {
    position: absolute;
    right: 100px;
    top: -55px;

}

@media screen and (min-width: 1920px) {

    .links {
        .container {
            display: flex;
            margin: 0;
            padding: 0 145px;

        }
    }
}
</style>