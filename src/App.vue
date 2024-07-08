<script>
import AppHeader from './components/AppHeader.vue'
import AppShop from './components/AppShop.vue'
import AppFooter from './components/AppFooter.vue'
import comicsList from './components/comicsList.vue';
import jumbotron from './components/jumbotron.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppShop,
    AppFooter,
    comicsList,
    jumbotron,
  }
}
</script>

<template>
    <body>
        <AppHeader />
        <main>
            <jumbotron/>
            <comicsList/>
        </main>
        <AppShop/>
        <AppFooter/>
    
    </body>
</template>
  

<style lang="scss">
body{
    background-color: rgb(33, 33, 33);
    margin: 0;
    padding-top: 20px;
}
</style>
