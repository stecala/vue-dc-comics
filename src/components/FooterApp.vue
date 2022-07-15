<template>
  <footer id="IDfooter">
    <FooterTop />
    <FooterBottom />
  </footer>
</template>

<script>
import FooterTop from './components-footer/TopFooter.vue'
import FooterBottom from './components-footer/BottomFooter.vue'

export default {
name : 'IDfooter',
components :{
    FooterTop,
    FooterBottom,
  }
}
</script>

<style>
</style>