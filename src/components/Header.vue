<template>
  <header>
    <Navbar />
    <Jumbotron />
  </header>
</template>

<script>
import Navbar from "./HeaderComponents/Navbar.vue";
import Jumbotron from "./HeaderComponents/Jumbotron.vue";

export default {
    components: {
    Navbar,
    Jumbotron
  },

}
</script>

<style>

</style>