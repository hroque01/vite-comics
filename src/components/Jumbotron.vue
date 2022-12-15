<script>
export default {
    data() {
        return {
            jumbotron: "/img/jumbotron.jpg"
        }
    }
}
</script>

<template>
    <section class="Jumbotron">
        <img :src="jumbotron" alt="">
    </section>
</template>


<style lang="scss" scoped>
.Jumbotron {
    height: 400px;

    img {
        height: 100%;
        width: 100%;
        object-fit: cover;
        object-position: 20% 0;
    }
}
</style>