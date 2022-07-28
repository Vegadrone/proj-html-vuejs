<template>
  <main>
    <section class="get-behind-the-wheel">
      <div class="container">
        <div class="row">
          <div class="col-6">
            <h2 class="fw-bold mt-5">Get Behind The Wheel</h2>
            <p class="fs-5 fw-light mt-4">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Aperiam,
              iusto nemo mollitia neque magnam architecto voluptas ad rerum.
            </p>
            <p class="fw-lighter">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Consequatur omnis quis impedit aperiam. Aliquam quis dolor
              reiciendis. Non aliquid, commodi, dicta quasi totam delectus
              voluptas, repellendus facilis optio voluptates cupiditate. Lorem
              ipsum, dolor sit amet consectetur adipisicing elit. Tempore cum
              necessitatibus eius nulla molestiae dicta recusandae inventore a
              ullam dolor saepe itaque, ut, reprehenderit labore voluptate nam
              voluptatem harum error!
            </p>
          </div>
          <div class="col-6">
            <Form />
          </div>
        </div>
      </div>
    </section>
    <section class="learn-to-drive-today">
      <div class="container">
        <div class="row">
          <div class="col-6 p-3">
            <h2 class="text-light fw-bold">Start Learning to Drive Today</h2>
            <p class="text-light fw-bold">
              Give us a call to schedule your first driving lesson
            </p>
          </div>
          <div class="col-6 p-3">
            <!-- this thing is copy pasted from header navbar, think of it -->
            <span class="text-light fs-3">
              <i class="fa-solid fa-phone-flip t"></i>
              1-800-555-555
            </span>
          </div>
        </div>
      </div>
    </section>
    <section class="services">
      <Services />
    </section>
    <section class="rate">
      <Rate />
    </section>
    <section class="instructors">
      <Instructors />
    </section>
    <section class="testimonials">
      <Testimonials />
    </section>
    <section class="latest-news">
      <LatestNews />
    </section>
    <section class="newsletter">
      <Newsletter />
    </section>
  </main>
</template>

<script>
import Form from "./MainComponents/Form.vue";
import Services from "./MainComponents/Services.vue";
import Rate from "./MainComponents/Rate.vue";
import Instructors from "./MainComponents/Instructors.vue";
import Testimonials from "./MainComponents/Testimonials.vue";
import LatestNews from "./MainComponents/LatestNews.vue";
import Newsletter from "./MainComponents/Newsletter.vue";

export default {
  name: "Main",

  components: {
    Form,
    Services,
    Rate,
    Instructors,
    Testimonials,
    LatestNews,
    Newsletter,
  },
};
</script>

<style lang="scss">
.learn-to-drive-today {
  background-image: url("../assets/siteAssets/horizontal-cta-background.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}

.services {
  background-image: url("../assets/siteAssets/promise-background.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}

.testimonials {
  background-image: url("../assets/siteAssets/testimonial-background.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}

.latest-news {
  background-image: url("../assets/siteAssets/latestnews-background.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}

.newsletter {
  background-image: url("../assets/siteAssets/newsletter_background.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  padding: 4rem 0rem;
}

.square-card {
  width: calc((100% / 3) - 2rem);
}
</style>