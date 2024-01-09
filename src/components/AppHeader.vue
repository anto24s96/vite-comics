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
                    <a href="#" :class="index == 1 ? 'active' : ''">
                        {{ link.label }}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>
<style lang="scss"scoped>
@use "../styles/partials/variables" as *;

header {
    justify-content: space-between;
    align-items: center;

    img {
        width: 100px;
    }

    ul {
        list-style-type: none;

        li {
            position: relative;

            a {
                text-decoration: none;
                color: #71777C;
                margin: 0 10px;
                text-transform: uppercase;
                font-weight: 600;
                line-height: 10;

                &.active,
                &:hover {
                    color: $blue_primary;

                    &::after {
                        content: "";
                        position: absolute;
                        bottom: 0;
                        left: 10px;
                        width: calc(100% - 20px);
                        height: 5px;
                        background-color: $blue_primary;
                    }
                }
            }
        }

    }
}
</style>