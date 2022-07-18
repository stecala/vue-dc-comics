<template>
    <div class="bg-foot position-relative"> 
        <div class="container-lg">
            <div class="row align-items-center">
                <div class="col-7 d-flex align-items-center">
                    <a class="mybtn">SING-UP NOW</a>
                </div>
                <div class="col-5 d-flex align-items-center justify-content-end">
                    <h3>FOLLOW US</h3>
                    <ul class="d-flex align-items-center mt-3">
                        <li v-for="(element, index) in socials" :key="index"><a :href='element.url'><img :src="`/img/${element.icon}`" alt="element.name"></a></li>
                    </ul>
                </div>
            </div>
        </div>
        <img src="https://www.dccomics.com/sites/default/files/files/character-pops/batman_char-pop_58910497bad9c5.66936402.png" alt="batman" class="myimg">
    </div>
</template>

<script>
export default {
    data: function () {
        return {
            socials: [
                {
                    name: "Facebook",
                    url: "#",
                    icon: "footer-facebook.png"
                },
                {
                    name: "Twitter",
                    url: "#",
                    icon: "footer-twitter.png"
                },
                {
                    name: "You Tube",
                    url: "#",
                    icon: "footer-youtube.png"
                },
                {
                    name: "Pinterest",
                    url: "#",
                    icon: "footer-pinterest.png"
                },
                {
                    name: "Periscope",
                    url: "#",
                    icon: "footer-periscope.png"
                }]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";

.bg-foot {
    background-color: $bgFooter;
    height: 87px;
}

.mybtn {
    border: 2px solid $primaryColor;
    padding: 10px;
    text-decoration: none;
    color: $textColorPrimary;
    font-size: 1.2rem;

    &:hover {
        cursor: pointer;
    }
}
h3{
    color: $primaryColor;
}
ul{
    padding: 0;
    list-style: none;
    li{
        margin: 10px;
    }
}
.myimg{
    position: absolute;
    top: -680px;
    right: 0;
}
</style>