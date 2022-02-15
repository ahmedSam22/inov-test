<template>
    <div class="main">
        <div class="dot-pattern"></div>
        <div class="main__slider">

        </div>

        <div class="bg-circle"></div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import url("../style/Global.scss");
.main{
    position: relative;
    padding : 20px;
    display: flex;
    justify-content: center;
    height: 700px;
    align-items: center;
    
    &__slider{
width: 846.89px;
height: 549.29px;
background: #8d5da7;
border-radius: 40px;
z-index: 1;
    }


}
.dot-pattern{
    position : absolute;
    left : 125px;
    top:15px

}

.bg-circle{
    position: absolute;
    right: 122px;
    bottom: -34px;
}
</style>