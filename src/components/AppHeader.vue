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
        <nav class="navbar">
            <figure>
                <img src="../assets/img/dc-logo.png" alt="dc_logo">
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
header {
    margin-top: 20px;
    min-height: 100px;

    .navbar {
        display: flex;
        align-items: center;
        justify-content: space-between;

    }

    figure {
        width: 85px;
    }

    ul {
        display: flex;
    }

    a {
        color: black;
    }

    a.active {
        color: #0182F9;
    }
}
</style>