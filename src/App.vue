<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';
  import ListCards from './components/ListCards.vue';
  import SingleCard from './components/SingleCard.vue';

  export default {
    components: {
      AppHeader,
      AppMain,
      AppFooter,
    }
  }
</script>

<template>
  <AppHeader/>
  <AppMain/>
  <AppFooter/>
</template>

<style lang="scss">
  @use './style/general.scss'
</style>