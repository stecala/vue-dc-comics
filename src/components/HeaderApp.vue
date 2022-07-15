<template>
  <div>
      <div class="container-lg">
          <div class="row py-4 ">
              <div class="col-5">
                  <img src="../assets/img/dc-logo.png" alt="Main logo DC">
              </div>
              <div class="col-7">

              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
  data: function(){
      return{
          navList : [
          {
            section : 'CHARACTERS',
            active : 'false',
            url : '#',
          },
          {
            section : 'COMICS',
            active : 'true',
            url : '#',
          },
          {
            section : 'MOVIE',
            active : 'false',
            url : '#',
          },
          {
            section : 'TV',
            active : 'false',
            url : '#',
          },
          {
            section : 'GAMES',
            active : 'false',
            url : '#',
          },
          {
            section : 'COLLECTIBLES',
            active : 'false',
            url : '#',
          },
          {
            section : 'VIDEOS',
            active : 'false',
            url : '#',
          },
          {
            section : 'FANS',
            active : 'false',
            url : '#',
          },
          {
            section : 'NEWS',
            active : 'false',
            url : '#',
          },
          {
            section : 'SHOP',
            active : 'false',
            url : '#',
          },
          ]
      }
  }
}

</script>

<style scoped lang="scss">

</style>
