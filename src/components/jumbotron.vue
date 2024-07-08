<script>
export default{
    name: "jumbotron",
}
</script>

<template>
    <div class="jumbotron">
        <div class="current-series">Current Series</div>
    </div>
</template>

<style lang="scss" scoped>
.jumbotron{
    max-width: 100%;
    height: 200px;
    background-image: url('https://www.games-galaxy.it/wp-content/uploads/2023/02/dc-comics-single-player-warner-bros-alla-ricerca-di-una-figura-professionale.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
}

.current-series{
    position: absolute;
    color: white;
    background-color: #0282F9;
    padding: 10px;
    bottom: -10%;
    left: 30%;
}
</style>