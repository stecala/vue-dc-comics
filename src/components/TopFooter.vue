<template>
    <div class="footer-container">
        <div class="container-lg">
            <div class="row">
                <div class="col-6"></div>
                <div class="col-6 img-bg">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data : function (){
        return{
        
        }
    }
}
</script>

<style lang="scss" scoped>
.footer-container {
    width: 100%;
    height: 500px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
}
.img-bg {
    background-image: url('../assets/img/dc-logo-bg.png');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    height: 500px;
}
</style>