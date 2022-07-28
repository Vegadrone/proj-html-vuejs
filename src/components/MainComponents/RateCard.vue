<template>
   <div class="square-wrapper">
    <div class="rate-card">
      <h1 class="text-center">{{percentRate}}</h1>
      <p class="text-center">{{rateType}}</p>
    </div>
</div>
</template>

<script>
export default {
   props:{
     percentRate: String,
    rateType: String,
   }

}
</script>

<style>

</style>