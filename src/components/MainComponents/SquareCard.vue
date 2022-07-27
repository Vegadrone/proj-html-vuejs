<template>
  <div class="square-wrapper">
    <h1 class="text-center">{{percentRate}}</h1>
    <p class="text-center">{{rateType}}</p>
  </div>
</template>

<script>
export default {
  props: {
    percentRate: String,
    rateType: String,
  },
};
</script>

<style lang="scss">
    .square-wrapper{
        border: 2px solid black;
    }
</style>