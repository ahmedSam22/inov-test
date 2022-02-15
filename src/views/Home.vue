<template>
<div class="container">
    <pageHeader />
        <Slider />

    <Cards />
</div>
<Footer/>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import pageHeader from "../components/Page-header.vue";
import Footer from "../components/Footer.vue";
import Cards from "../components/Cards.vue";
import Slider from "../components/body.vue";

export default defineComponent({
  name: "Home",

  components: {
    pageHeader,
    Footer,
    Cards,
    Slider
  },
});
</script>
