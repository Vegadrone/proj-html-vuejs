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
  padding: 3rem 0rem;
  }

  .socials-bar{
    background-color: $footerBgColor ;
    padding: 1rem 0rem;
  }
</style>