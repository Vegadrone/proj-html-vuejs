<template>
  <div class="service-card">
    <img :src="require(`../../assets/siteAssets/${imgPath}`)" :alt="imgPath">
    <h6>{{serviceName}}</h6>
    <button class="btn btn-success">{{buttonText}}</button>
  </div>
</template>

<script>

export default {
  props:{
    imgPath:String,
    serviceName:String,
    buttonText:String
  }

}
</script>

<style lang="scss">
  .service-card{
    border:2px solid black
  }
</style>