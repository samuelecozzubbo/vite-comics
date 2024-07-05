<script>
import AppHeader from './components/AppHeader.vue'
import AppShop from './components/AppShop.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppShop,
    AppFooter,
  }
}
</script>

<template>
    <body>
        <AppHeader />
        <main>
            Parte centrale
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
main{
    background-color: black;
    width: 100%;
    min-height: 100px;
    color: white;
}
</style>
