<template>
    <main>
        <jumbo/>
        <div class="container">
            <cards/>
        </div>
    </main>
</template>

<script>
import cards from '../components/sections/cards.vue';
import jumbo from '../components/sections/jumbo.vue';

export default {
    name: 'Main',
    components: {
        cards,
        jumbo,
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';
    main{
        background-color: $darkGray;
        
    }
    // h1{
    //     color: white;
    //     padding: 50px 0;
    // }
</style>