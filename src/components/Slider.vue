<template>
<div id="carouselExampleCaptions" data-bs-interval="2000"  class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="../assets/bg.jpg"  class="d-block h-100" alt="...">


    </div>
    <div class="carousel-item">

    </div>
    <div class="carousel-item p-5 " >
      <img src="../assets/bg.jpg" style="border-radius:40px" class="d-block  w-100 h-100" alt="...">
    
    </div>
  </div>
</div>
</template>

<script>
  export default {
   
    methods: {
   
    }
  }
</script>
<style lang="scss" scoped>
.carousel-item{
    position: relative;
    object-fit:contain;
    img{
        height: 100%;
    }
    &__label{
    position: absolute;
    background-color: red;
}
}

</style>