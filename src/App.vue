<script>
import AppHeader from './components/AppHeader.vue'
import AppShop from './components/AppShop.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppShop,
  }
}
</script>

<template>
  <AppHeader />
  <main>
    Parte centrale
  </main>
  <AppShop/>
</template>

<style lang="scss">
main{
    background-color: black;
    width: 100%;
    min-height: 100px;
    color: white;
}
</style>
