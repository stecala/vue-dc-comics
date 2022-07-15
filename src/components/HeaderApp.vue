<template>
  <div>
      <div class="container-lg">
          <div class="row py-4 ">
              <div class="col-5">
                  <img src="../assets/img/dc-logo.png" alt="Main logo DC">
              </div>
              <nav class="col-7 d-flex align-items-center justify-content-center">
                  <ul class="fw-bolder d-flex">
                      <li v-for="(element, index) in navList" :key="index" class="px-2" :class="{active : element.active == true}">
                          {{element.section}}
                      </li>
                  </ul>
              </nav>
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
  ul{
    list-style: none;
    li{

      &:hover{
        cursor: pointer;
      }
    }
  }
  .active{
    border-bottom: 2px solid rgb(12,124,236);
    color: rgb(12,124,236);
  }
</style>
