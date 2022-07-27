<template>
  <div>
    <img :src="require(`../../assets/siteAssets/${imgPath}`)" :alt="imgPath">
    <h3 class="fw-bold">{{serviceName}}</h3>
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

</style>