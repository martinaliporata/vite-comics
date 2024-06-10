<script>
  export default {
    data() {
      return {
        navbarHeader: [
          {
            name: 'characters',
            link: '#',
            active: false,
          },
          {
            name: 'comics',
            link: '#',
            active: true,
          },
          {
            name: 'movies',
            link: '#',
            active: false,
          },
          {
            name: 'tv',
            link: '#',
            active: false,
          },
          {
            name: 'games',
            link: '#',
            active: false,
          },
          {
            name: 'collectibles',
            link: '#',
            active: false,
          },
          {
            name: 'videos',
            link: '#',
            active: false,
          },
          {
            name: 'fans',
            link: '#',
            active: false,
          },
          {
            name: 'news',
            link: '#',
            active: false,
          },
          {
            name: 'shop',
            link: '#',
            active: false,
          }
        ]
      }
    }
  }
</script>

<template>
    <section class="logo">
      <img src="../assets/img/dc-logo.png" alt="">
    </section>
    <section>
      <nav>
        <ul>
          <li v-for="element in navbarHeader" :key="index">
            {{ element.name }}
          </li>
        </ul>
      </nav>
    </section>
</template>

<style lang="scss" scoped>
    @use '../style/partials/variables' as *;
    @use '../style/partials/mixins' as *;
</style>
