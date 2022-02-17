<template>
     <UpperBody class="mb-5" />
     <LowerBody class="mt-5" />
  
</template>

<script>  
  import UpperBody from './Upper-body.vue';
  import LowerBody from './Lower-body.vue';
export default {
components:{
    UpperBody,
    LowerBody,
}
};
</script>
<style lang="scss" scoped>
div{
  display: grid;
  gap: 50px;
}
</style>