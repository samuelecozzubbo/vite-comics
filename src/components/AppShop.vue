<script>
export default {
    name: 'AppShop',
    data() {
        return {
            links: [
                {
                    text: "DIGITAL COMICS",
                    imgUrl: "../assets/img/buy-comics-digital-comics.png",
                    current: false,
                },
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <ul>
                <li v-for="(link,index) in links" :key="index">
                    <img :src="link.imgUrl" alt="img">
                </li>
            </ul>

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/mixings' as *;

section{
    background-color: #0282F9;
    max-width: 100%;
    min-height: 50px;
}

.container{
    @include center(space-between)
}
</style>