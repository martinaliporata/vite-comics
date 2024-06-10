<script>
    export default {
        data() {
            return {
                navbarDcComics: [
                    {
                        name: 'Characters',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Comics',
                        link: '#',
                        active: true,
                    },
                    {
                        name: 'Movies',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'TV',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Games',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'News',
                        link: '#',
                        active: false,
                    }
                ],
                navbarShop: [
                    {
                        name: 'Shop DC',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Shop DC Collectibles',
                        link: '#',
                        active: false,
                    },
                ],
                navbarDc: [
                    {
                        name: 'Terms of Use',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Privacy policy (New)',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Ad Choices',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Advertising',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Jobs',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Subscriptions',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Talent Workshops',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'CPSC Certificates',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Ratings',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Shop Help',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'Contact Us',
                        link: '#',
                        active: false,
                    }
                ],
                navbarSites: [
                    {
                        name: 'DC',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'MAD Magazine',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'DC Kids',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'DC Universe',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'DC Power Visa',
                        link: '#',
                        active: false,
                    }
                ]
            }
        }
    }
</script>

<template>
    <main>
        <section class="main-div">
            <h1>
                <-- Contents goes here -->
            </h1>
        </section>
        <section class="navbar-main">
            <section class="navbar-left">
                <h2>
                    dc comics
                </h2>
                <nav>
                    <ul>
                        <li v-for="element in navbarDcComics" :key="index">
                            {{ element.name }}
                        </li>
                    </ul>
                </nav>
                <h2>
                    shop
                </h2>
                <nav>
                    <ul>
                        <li v-for="element in navbarShop" :key="index">
                            {{ element.name }}
                        </li>
                    </ul>
                </nav>
            </section>
            <section class="navbar-middle">
                <h2>
                    dc
                </h2>
                <nav>    
                    <ul>
                        <li v-for="element in navbarDc" :key="index">
                            {{ element.name }}
                        </li>
                    </ul>
                </nav>
            </section>
            <section class="navbar-right">
                <h2>
                    sites
                </h2>
                <nav>    
                    <ul>
                        <li v-for="element in navbarSites" :key="index">
                            {{ element.name }}
                        </li>
                    </ul>
                </nav>
            </section>
        </section>
    </main>
</template>

<style lang="scss" scoped>
    @use '../style/partials/variables' as *;
    @use '../style/partials/mixins' as *;

    main {
        background-image: url(../assets/img/footer-bg.jpg);
        background-position: center;
        background-size: contain;
        background-repeat: repeat;
        margin: 0 auto;
    }

    h2 {
        @include text-uppercase;
    }

    .main-div {
        height: 15vh;
        background-color: #1c1c1c;
        @include flex-row;
    }

    h1,h2 {
        color: $color-white;
    }

    li {
        color: $color-grey;
    }

    .navbar-main {
        @include flex-row;
        align-items: baseline;
    }

    .navbar-left,
    .navbar-middle,
    .navbar-right {
        padding-left: 1rem;
    }

</style>