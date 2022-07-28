<template>
    <div class="instructors-card">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <img :src="require(`../../assets/siteAssets/${img}`)" :alt="img" />
            <h6 class="fw-bold">{{ name }}</h6>
            <p>{{ text }}</p>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  props: {
    img: String,
    name: String,
    text: String,
  },
};
</script>

<style lang="scss">
.square-wrapper {
  border: 2px solid black;
}
</style>