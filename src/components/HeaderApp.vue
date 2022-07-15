<template>
  <header>
      <div class="container-lg">
          <div class="row">
              <div class="col-4 d-flex align-items-center">
                  <img src="../assets/img/dc-logo.png" alt="Main logo DC">
              </div>
              <nav class="col-8 d-flex align-items-center ">
                  <ul class="fw-bolder d-flex justify-content-between">
                      <li v-for="(element, index) in navList" :key="index" class="me-4 py-5" :class="{active : element.active == 'true'}">
                          {{element.section}}
                      </li>
                  </ul>
              </nav>
          </div>
      </div>
  </header>
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
  @import "../assets/style/variables.scss";

  ul{
    list-style: none;
    margin-bottom: 0;
    li{

      &:hover{
        cursor: pointer;
      }
    }
  }
  .active{
    border-bottom: 5px solid $primaryColor;
    color: $primaryColor;
  }
  
</style>
