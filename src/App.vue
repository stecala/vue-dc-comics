<template>
  <div id="app">
    <HeaderApp />
    <MainContentApp />
    <NavMain />
    <FooterApp />
  </div>
</template>

<script>
import HeaderApp from './components/HeaderApp.vue'
import MainContentApp from './components/MainContentApp.vue'
import FooterApp from './components/FooterApp.vue'
import NavMain from './components/NavMain.vue'

export default {
  name: 'app',
  components :{
    HeaderApp,
    MainContentApp,
    FooterApp,
    NavMain,
  }
}
</script>

<style lang="scss">
    @import "~bootstrap/dist/css/bootstrap.css";

</style>
