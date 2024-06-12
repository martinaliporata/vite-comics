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
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Youtube',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Pinterest',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Periscope',
                        link: '#',
                        active: false,
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
            <div>
                <img src="../assets/img/footer-periscope.png" alt="">
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
