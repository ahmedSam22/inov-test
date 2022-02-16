<template>
<div class="container-fluid p-0">
  <div class="col-md-12">
    <pageHeader />
  </div>
    <div class="col-md-12 mb-5">
      <Body />
    </div>
    <div class="col-md-12 mt-5 mb-5">
      <Cards />
    </div>
    <div class="col-md-12">
      <Footer/>
    </div>
        
    
</div>

</template>
<style lang="scss" scoped>
.container-fluid{
display: grid;
  gap: 50px;}
</style>

<script lang="ts">
import { defineComponent } from "vue";
import pageHeader from "../components/Page-header.vue";
import Footer from "../components/Footer.vue";
import Cards from "../components/Cards.vue";
import Body from "../components/body.vue";

export default defineComponent({
  name: "Home",

  components: {
    pageHeader,
    Footer,
    Cards,
    Body
  },
});
</script>
