<template>
    <section>
        <div class="jumbotron">
            <img src="../../assets/img/jumbotron.jpg" alt="">
        </div>
    </section>
</template>

<script>
export default {
    name: 'jumbo'
}
</script>

<style lang = "scss" scoped>
    section {
        height: 320px;
        .jumbotron {
            height: 100%;
            img {
                width: 100%;
                height: 100%;
                object-fit: cover;
                object-position: top;
            }
        }
    }
</style>