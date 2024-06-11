<script>
    export default {
        data() {
            return {
                
            }
        },
        props : {
            card: {
                type: Object,
                required: true,
            }
        }
    }
</script>

<template>
    <section class="cards-list">
        <article>
            <img :src="card.thumb" alt="card.series">
            <h4>
                {{ card.series }}
            </h4>
        </article>
    </section>
</template>

<style lang="scss" scoped>
    @use '../style/partials/variables' as *;
    @use '../style/partials/mixins' as *;

</style>