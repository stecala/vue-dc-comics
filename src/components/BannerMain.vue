<template>
  <div class="banner-main">
      <img :src="imagesList[active]" >
  </div>
</template>

<script>
export default {
  data : function() {
    return {
      active : 0,
      imagesList : [
      '/img/jumbotron.jpg',
      'https://www.dccomics.com/sites/default/files/dc-hero_20220715_GreenLanternDocClip_62d1efcb0dba15.96911971.jpg',
      'https://www.dccomics.com/sites/default/files/dc-hero_20220715_SGWOT_62d1ef85872b78.55046194.jpg'
      ]
    }
  },
  methods: {
    changeActive(){
      this.active++
      if(this.active === this.imagesList.length){
        this.active = 0
      }    
    },
    startInterval(){
          setInterval(this.changeActive, 4000)
    }
  },
  created (){
      this.startInterval()
  } 
}
</script>

<style scoped lang="scss">
.banner-main{
  height: 70vh;
  width: 100%;
  img{
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top;
  }
}


</style>