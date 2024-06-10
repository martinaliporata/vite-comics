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
                        name: 'Movies',
                        link: '#',
                        active: true,
                    },
                    {
                        name: 'comics',
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
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'news',
                        link: '#',
                        active: false,
                    }
                ],
                navbarShop: [
                    {
                        name: 'shop DC',
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
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    }
                ],
                navbarSites: [
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    },
                    {
                        name: 'videos',
                        link: '#',
                        active: false,
                    }
                ]
            }
        }
    }
</script>

<template>
    <section>
        <nav>
            <ul>
                <li v-for="element in navbarDcComics" :key="index">
                    {{ element.name }}
                </li>
            </ul>
            <ul>
                <li v-for="element in navbarShop" :key="index">
                    {{ element.name }}
                </li>
            </ul><ul>
                <li v-for="element in navbarDc" :key="index">
                    {{ element.name }}
                </li>
            </ul><ul>
                <li v-for="element in navbarSites" :key="index">
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