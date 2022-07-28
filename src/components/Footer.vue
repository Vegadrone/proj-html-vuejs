<template>
  <footer>
    <section class="contacts-and-courses">
      <ContactsAndCourses />
    </section>
    <section class="socials-bar">
      <SocialsBar />
    </section>
  </footer>
</template>

<script>
import ContactsAndCourses from "./FooterComponents/ContactsAndCourses.vue";
import SocialsBar from "./FooterComponents/SocialsBar.vue";
export default {
  components: {
    ContactsAndCourses,
    SocialsBar,
  },
};
</script>

<style lang="scss">

@import "../style/variables.scss";
  .contacts-and-courses{
  background-image: url("../assets/siteAssets/footer-background-color.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  }

  .socials-bar{
    background-color: $footerBgColor ;
    height: 100px;
    width: 100%;
  }
</style>