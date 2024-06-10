<script>
    export default {
        data() {
            return {
                navbarShop: [
                    {
                        name: 'Facebook',
                        img: url(./assets/img/footer-facebook.png)
                        link: '#',
                        active: false,
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
            <nav>
            <ul>
                <li v-for="element in navbarFooter" :key="index">
                {{ element.img }}
                </li>
            </ul>
            </nav>
        </section>
    </header>
</template>

<style lang="scss" scoped>
    @use '../style/partials/variables' as *;
    @use '../style/partials/mixins' as *;

    footer {
        height: 15vh;
        @include text-uppercase;
    }

    button,
    h2 {
        @include text-uppercase;
    }
</style>
