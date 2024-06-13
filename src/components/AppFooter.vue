<script>
    export default {
        data() {
            return {
                navbarSocial: [
                    {
                        name: 'Facebook',
                        image:'../assets/img/footer-facebook.jpg'
                    },
                    {
                        name: 'Twitter',
                        image:'../assets/img/footer-twitter.jpg'
                    },
                    {
                        name: 'Youtube',
                        image:'../assets/img/footer-youtube.jpg'
                    },
                    {
                        name: 'Pinterest',
                        image:'../assets/img/footer-pinterest.jpg'
                    },
                    {
                        name: 'Periscope',
                        image:'../assets/img/footer-periscope.jpg'
                    },
                ]
            }
        }
    }
</script>

<template>
    <header>
        <section class="button">
            <button>
                sign-up now!
            </button>
        </section>
        <section class="navbar">
            <h2>
                follow us
            </h2>
            <div v-for="element in navbarSocial" :key="index">
                {{element.image}}
            </div>
        </section>
    </header>
</template>

<style lang="scss" scoped>
    @use '../style/partials/variables' as *;
    @use '../style/partials/mixins' as *;

    footer {
        height: 15vh;
        @include text-uppercase;
        background-color: #303030;
    }

    button,
    h2 {
        @include text-uppercase;
    }
</style>
