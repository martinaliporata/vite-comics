<script>
    import SingleCard from './SingleCard.vue'
    export default {
        data() {
            return {
                
            }
        }
    }
</script>

<template>
    <section class="cards-list">
        <img :src="card.thumb" alt="card.series">
        <h4>
            {{ card.series }}
        </h4>
    </section>
</template>

<style lang="scss" scoped>
    @use '../style/partials/variables' as *;
    @use '../style/partials/mixins' as *;

    h1 {
        @include text-uppercase;
    }
</style>