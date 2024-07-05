<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false,
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true,
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false,
                },
                {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false,
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false,
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false,
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false,
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false,
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false,
                },

            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <a href="/" class="brand">
            <img src="../assets/img/dc-logo.png"
                alt="logo">
        </a>

        <!-- Navigazione -->
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :class="{ active: link.current }" :href="link.url">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
        </div>
        
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/mixings' as *;

.container,ul{
    @include center(space-between);
}

ul{
    gap: 12px;
    list-style: none;

    a{
        text-decoration: none;
        color: #55595C;
    }
}


</style>