<script>
export default{
    name: "card",
    props: {
        details: Object,
    }
}
</script>

<template>
    <div class="prod-card">
        <img :src="details.thumb" alt="descrizione altenativa">
         <h3>{{ details.series }}</h3>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/mixings' as *;

.prod-card{
    flex-basis: calc(100% / 6 - 30px);
    margin-bottom: 20px;
    h3{
        color: rgb(209, 209, 209);
        font-size: 0.9em;
        margin-top: 10px;
    }

    img{
        display: block;
        aspect-ratio: 1;
        object-fit: cover;
    }
}
</style>