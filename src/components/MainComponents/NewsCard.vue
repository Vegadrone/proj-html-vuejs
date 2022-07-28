<template>
  <div>
    <img :src="require(`../../assets/siteAssets/${img}`)" :alt="img">
    <h2>{{ title }}</h2>
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

<style>
</style>