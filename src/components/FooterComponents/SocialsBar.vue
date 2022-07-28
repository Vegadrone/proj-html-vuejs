<template>
  <div class="container">
    <div class="row d-flex justify-content-between">
      <div class="col-6">
        <span>©Copyright 2012 - 2020 | Avada Theme by <span class="accent">ThemeFusion</span> | All Rights Reserved | Powered by <span class="accent">WordPress</span></span>
      </div>
      <div class="col-6 text-light text-center"><i class="fa-brands fa-facebook-f"></i><i class="fa-brands fa-twitter"></i><i class="fa-brands fa-youtube"></i><i class="fa-brands fa-instagram"></i></div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";
span{
  color:$secondaryColor;
  font-size: 0.8rem;
}

i{
  margin: 0 1rem;
}
.accent{
  color: $brandColor;
}

</style>