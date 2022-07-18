<template>
  <div class="col-2">
        <div class="img-container">
            <img :src="card.thumb" :alt="card.series">
        </div>
        <div class="text-container py-2">
            {{card.series}}
        </div>
  </div>
</template>

<script>
export default {
    props:{
        'card' : Object
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
div{
    cursor: pointer;
    .img-container{
        width: 192px;
        height: 200px;
        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }
    }
    .text-container{
        color: $textColorPrimary;
        text-transform: uppercase;
    }
}

</style>