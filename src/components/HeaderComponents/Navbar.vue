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
          <div class="col-12 d-flex justify-content-around">
            <img
              src="../../assets/siteAssets/avada-drivers-logo-2x-300x58.png"
              alt="logo"
            />
            <ul>
              <li v-for="(navBarEl, index) in navBarVoices" :key="index">
                <a class="text-uppercase fw-bold" href="">{{
                  navBarEl.button
                }}</a>
              </li>
            </ul>
            <button class="btn btn-success text-uppercase">book now</button>
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

<style lang="scss">
.up-nav-bar {
  background-color: #484848;

  span {
    color: #e5e8eb;
  }
}

.nav-bar {

background-color: #484848;

  ul {
    list-style: none;

    li {
      display: inline-block;
      padding: 1.5rem;

      a {
        color: #ffffff;
        text-decoration: none;
      }
    }
  }
}
</style>