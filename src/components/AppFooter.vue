<script>
export default {
    data() {
        return {
            socials: [
                "img/footer-facebook.png",
                "img/footer-twitter.png",
                "img/footer-youtube.png",
                "img/footer-pinterest.png",
                "img/footer-periscope.png"
            ]
        }
    }
}
</script>

<template>
    <section class="footer">
        <div class="container">
            <div class="btn">
                <h1>SIGN-UP NOW!</h1>
            </div>
            <div class="socials-part">
                <h1>FOLLOW US</h1>
                <ul>
                    <li v-for="social in socials">
                        <a href="#">
                            <img :src="social" alt="">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../temp/partials/mixins.scss' as *;
@use '../temp/partials/variables.scss' as *;

.footer {
    background-color: #303030;
    padding: 40px;

    .container {
        display: flex;
        align-items: center;
        justify-content: space-between;

        .socials-part {
            display: flex;
            align-items: center;

            h1 {
                color: $secondary;
                padding-right: 20px;
            }
        }

        .btn {
            border: 5px solid $secondary;
            padding: 10px;

            h1 {
                color: white;
            }
        }

    }

    ul {
        display: flex;

        li {
            list-style: none;
            padding-left: 10px;
            padding-right: 10px;
        }
    }


}
</style>