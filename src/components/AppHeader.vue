<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    label: "Characters",
                    url: "#",
                    current: false,
                },
                {
                    label: "Comics",
                    url: "#",
                    current: false,
                },
                {
                    label: "Movies",
                    url: "#",
                    current: true,
                },
                {
                    label: "Tv",
                    url: "#",
                    current: false,
                },
                {
                    label: "Games",
                    url: "#",
                    current: false,
                },
                {
                    label: "Collectibles",
                    url: "#",
                    current: false,
                },
                {
                    label: "Videos",
                    url: "#",
                    current: false,
                },
                {
                    label: "Fans",
                    url: "#",
                    current: false,
                },
                {
                    label: "News",
                    url: "#",
                    current: false,
                },
                {
                    label: "Shop",
                    url: "#",
                    current: false,
                },

            ]
        }
    },
}
</script>
<template lang="">
    <header class="container d-flex">
        <a href="#">
            <img src="../assets/img/dc-logo.png" alt="logo_header">
        </a>
        <nav>
            <ul class="d-flex">
                <li v-for="(link, index) in links" :key="index">
                    <a href="#">
                        {{ link.label }}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>
<style lang="scss"scoped>
header {
    height: 150px;
    justify-content: space-between;
    align-items: center;

    img {
        width: 100px;
    }

    ul {
        list-style-type: none;

        li a {
            text-decoration: none;
            color: #71777C;
            margin: 0 10px;
            text-transform: uppercase;
            font-weight: 600;
        }
    }
}
</style>