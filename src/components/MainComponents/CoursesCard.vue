<template>
  <div>
    <img :src="img" :alt="imgAlt">
    <h3 class="fw-bold">{{name}}</h3>
    <button class="btn btn-success">{{btn}}</button>
  </div>
</template>

<script>

export default {
  props:{
    img:String,
    name:String,
    imgAlt:String,
    btn:String
  }

}
</script>

<style lang="scss">

</style>