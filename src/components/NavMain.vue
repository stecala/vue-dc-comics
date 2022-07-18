<template>
    <div class="bg-container-nav-main d-flex">
        <div class="container-lg d-flex justify-content-between ">
            <div v-for="(element, index) in navMainList" :key="index" class="d-flex align-items-center">
                <div class="img-container">
                    <img :src="`/img/${element.src}`">
                </div>
                <div class="mytxt ps-2">{{element.txt}}</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data: function () {
        return {
            navMainList: [
                {
                    src: 'buy-comics-digital-comics.png',
                    txt: 'DIGITAL COMICS',
                },
                {
                    src: 'buy-comics-merchandise.png',
                    txt: 'DC MERCHANDISE',
                },
                {
                    src: 'buy-comics-subscriptions.png',
                    txt: 'SUBSCRIPTION',
                },
                {
                    src: 'buy-comics-shop-locator.png',
                    txt: 'COMIC SHOP LOCATOR',
                },
                {
                    src: 'buy-dc-power-visa.svg',
                    txt: 'DC POWER VISA',
                },

            ]

        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
img{
    width: 100%;
    height: 100%;
}
.bg-container-nav-main {
    background-color: $primaryColor;
    height: 150px;
    .container-lg:hover{
        cursor: pointer;
    }
}
.img-container{
    width: 50px;
    height: 50px;
}
.mytxt{
    color: $textColorPrimary;
    width: 200px;
}
</style>