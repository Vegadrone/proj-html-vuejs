<template>
  <div class="container">
    <div class="row">
      <div class="col-12 text-center">
        <img
          class="testimonials-thumb"
          :src="require(`../../assets/siteAssets/${img}`)"
          :alt="img"
        />
        <p>{{ text }}</p>
        <h6 class="fw-bold">{{ name }}</h6>
        <i
          class="fa-regular fa-circle mx-2"
          v-for="(n, index) in 5"
          :key="index"
        ></i>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    img: String,
    text: String,
    name: String,
  },
};
</script>

<style lang="scss" scoped>
</style>