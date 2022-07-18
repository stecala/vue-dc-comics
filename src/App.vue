<template>
  <div id="app">
    <HeaderApp />
    <BannerMain />
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
import BannerMain from './components/BannerMain.vue'

export default {
  name: 'app',
  components :{
    HeaderApp,
    MainContentApp,
    FooterApp,
    NavMain,
    BannerMain,
  }
}
</script>

<style lang="scss">
    @import "~bootstrap/dist/css/bootstrap.css";

</style>
