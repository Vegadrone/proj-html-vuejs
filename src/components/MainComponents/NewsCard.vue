<template>
  <div class="d-flex flex-column align-items-between text-center">
    <div class="news-img">
      <img class="w-100" :src="require(`../../assets/siteAssets/${img}`)" :alt="img">
    </div>
    <h4>{{ title }}</h4>
    <div>
        <span>{{date}}</span> | <span>{{comments}}</span>
    </div>
    <p>{{text}}</p>
  </div>
</template>

<script>
export default {
  name: "NewsCard",

  props: {
    img: String,
    title: String,
    date: String,
    comments: String,
    text: String,
  },
};
</script>

<style lang="scss">
@import "../../style/variables.scss";

.news-img{
  width: 15rem;
}

h4{
 color:$brandColor;
}
</style>