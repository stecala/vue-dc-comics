<template>
  <footer id="IDfooter">
    <FooterTop />
    <FooterBottom />
  </footer>
</template>

<script>
import FooterTop from './TopFooter.vue'
import FooterBottom from './BottomFooter.vue'

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