<template>
  <nav>
    <div class="up-nav-bar">
      <div class="container">
        <div class="row">
          <div class="col-12 d-flex justify-content-between">
            <span>We have a 95% Successful Pass Rate!</span>
            <span
              ><i class="fa-solid fa-phone-flip"></i>Give us a call to book yout
              tuition! 1-800-555-555</span
            >
          </div>
        </div>
      </div>
    </div>
    <div class="nav-bar">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <ul v-for="(navBarEl, index) in navBarVoices" :key="index">
              <li>{{navBarEl.button}}</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data: function () {
    return {
      navBarVoices: [
        {
          button: "Home",
          link: "#",
        },
        {
          button: "About",
          link: "#",
        },
        {
          button: "Prices",
          link: "#",
        },
        {
          button: "Courses",
          link: "#",
        },
        {
          button: "Locations",
          link: "#",
        },
        {
          button: "Blog",
          link: "#",
        },
      ],
    };
  },
};
</script>

<style>
</style>