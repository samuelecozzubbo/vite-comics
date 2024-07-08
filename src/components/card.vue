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
    text-align: center;
    flex-basis: calc(100% / 6);
    border: 2px solid lighten(white,70%);
    h3{
        color: white;
    }

    img{
        display: block;
        width: 100px;
        height: 100px; 
        object-fit: cover; 
        margin: 0 auto; 
    }
}
</style>