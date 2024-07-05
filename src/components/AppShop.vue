<script>
export default {
    name: 'AppShop',
    data() {
        return {
            links: [
                {
                    text: "DIGITAL COMICS",
                    imgUrl: "/img/buy-comics-digital-comics.png",
                    current: false,
                },
                {
                    text: "DC MERCHANDISE",
                    imgUrl: "/img/buy-comics-merchandise.png",
                    current: false,
                },
                {
                    text: "SUBSCRIPTION",
                    imgUrl: "/img/buy-comics-subscriptions.png",
                    current: false,
                },
                {
                    text: "COMIC SHOP LOCATOR",
                    imgUrl: "/img/buy-comics-shop-locator.png",
                    current: false,
                },
                {
                    text: "DC POWER VISA",
                    imgUrl: "/img/buy-dc-power-visa.svg",
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
                    <div class="img-container">
                        <img :src="link.imgUrl" alt="img">
                    </div>
                    <span>{{ link.text }}</span>
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
    @include center(horizontal);
    padding: 30px 0;
    
    ul{
        width: 100%;
       @include center(space-between);
    }

    li{
       @include center(horizontal);

    }

    .img-container{
        width: 40px;
    }
}

</style>