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
            <p>
                <-- Contents goes here -->
            </p>
        </section>
        <section class="navbar">
            <h5>
                dc comics
            </h5>
            <nav>
                <ul>
                    <li v-for="element in navbarDcComics" :key="index">
                        {{ element.name }}
                    </li>
                </ul>
            </nav>
            <h5>
                shop
            </h5>
            <nav>
                <ul>
                    <li v-for="element in navbarShop" :key="index">
                        {{ element.name }}
                    </li>
                </ul>
            </nav>
            <h5>
                dc
            </h5>
            <nav>    
                <ul>
                    <li v-for="element in navbarDc" :key="index">
                        {{ element.name }}
                    </li>
                </ul>
            </nav>
            <h5>
                sites
            </h5>
            <nav>    
                <ul>
                    <li v-for="element in navbarSites" :key="index">
                        {{ element.name }}
                    </li>
                </ul>
            </nav>
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
        background-repeat: no-repeat;
    }

    h5 {
        text-transform: uppercase;
    }

    .main-div {
        height: 25vh;
        background-color: #1c1c1c;
    }

    p,h5 {
        color: $color-white;
    }
</style>