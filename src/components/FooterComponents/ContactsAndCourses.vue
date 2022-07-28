<template>
  <div class="container">
    <div class="row">
      <div class="col-12 d-flex justify-content-between">
        <div class="brand">
          <img
            src="../../assets/siteAssets/avada-drivers-logo-1x.png"
            alt="logo"
          />
          <p>
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Veritatis
            alias fugiat ad sit fugit minus, quibusdam dignissimos nemo
            cupiditate explicabo, quos eligendi fuga! Maxime fugiat iusto beatae.
          </p>
        </div>

        <div>
          <h4 class="text-light text-uppercase">contacts</h4>
          <ul
            v-for="contactsMenuVoice in contactsMenuVoices"
            :key="contactsMenuVoice.id"
          >
            <li class="contacts-voices">
              {{ contactsMenuVoice.text }}
            </li>
          </ul>
        </div>
        <div>
          <h4 class="text-light text-uppercase">courses</h4>

          <ul
            class="courses-voices"
            v-for="(coursesMenuVoice, index) in coursesMenuVoices"
            :key="index"
          >
            <li class="courses-voices">
              <span class="mx-2"
                ><i class="fa-solid fa-circle-arrow-right"></i
              ></span>
              <span>{{ coursesMenuVoice.text }}</span>
            </li>
          </ul>
        </div>
        <div class="img-container">
          <img
            src="../../assets/siteAssets/footer-ad-grid-200x178.png"
            alt="ad-grid.png"
          />
          <button class="btn btn-success text-uppercase">book now</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      contactsMenuVoices: [
        {
          id: 1,
          text: "12345 Nort Main Street, NY 555555",
        },
        {
          id: 2,
          text: "1.800.555.6789",
        },
        {
          iid: 3,
          text: "info@your-domain.com",
        },
        {
          id: 4,
          text: "Theme-Fusion.com",
        },
      ],

      coursesMenuVoices: [
        {
          text: "Pass Plus",
        },
        {
          text: "Intensive Course",
        },

        {
          text: "Automatic",
        },

        {
          text: "Instructor Training",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";
p {
  color: $secondaryColor;
}

ul {
  list-style: none;
  padding:0;
  margin: 1rem 0;
  font-size: 0.8rem;


  .courses-voices {
    color: $brandColor;
  }

  .contacts-voices {
    color: $secondaryColor;
  }
}

.brand{
    width: 15rem;
    font-size: 0.8rem;
}

button{
    display: block;
    margin: 0 auto;
    margin-top: 1rem;
}
</style>