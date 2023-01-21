<script>
export default {
    name: "AppHeader",
    data() {
        return {
            // array oggetti navbar
            links: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                },
            ],
        }
    }
};
</script>

<template>
    <header class="container">
        <!-- header navbar -->
        <nav class="navbar">
            <figure>
                <a href="#"><img src="../assets/img/dc-logo.png" alt="dc_logo"></a>
            </figure>
            <ul>
                <li v-for="link in links" :key="link.text"><a :href="link.url" :class="{ 'active': link.current }">{{
                    link.text
                }}</a></li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
// importo file scss
@use '../assets/scss/partials/mixins' as *;
@use '../assets/scss/partials/variables' as *;

header {
    height: 120px;

    // header navbar
    .navbar {
        height: 100%;
        @include flex-between;

        figure {
            width: 85px;
            height: 85px;

            a {
                padding: 0;
            }
        }

        ul {
            display: flex;

            a {
                padding: 0 15px;
                display: block;
                color: black;
                font-weight: bold;

                &.active,
                &:hover {
                    color: $darkblue;
                }
            }

        }
    }
}
</style>