<template>
  <main>
   <section class="get-behind-the-wheel">
     <div class="container">
      <div class="row">
        <div class="col-6">
          <h2 class="fw-bold mt-5">Get Behind The Wheel</h2>
          <p class="fs-5 fw-light mt-4">Lorem ipsum dolor sit amet consectetur adipisicing elit. Aperiam, 
            iusto nemo mollitia neque magnam architecto voluptas ad rerum.</p>
            <p class="fw-lighter">Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur omnis quis impedit aperiam. 
              Aliquam quis dolor reiciendis. 
              Non aliquid, commodi, dicta quasi totam delectus voluptas, repellendus facilis optio voluptates cupiditate.
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Tempore cum necessitatibus eius nulla molestiae dicta recusandae 
              inventore a ullam dolor saepe itaque, ut, reprehenderit labore voluptate nam voluptatem harum error!</p>
        </div>
        <div class="col-6">
          <Form/>
        </div>
      </div>
    </div>
   </section>
   <section class="learn-to-drive-today">
    <div class="container">
      <div class="row">
        <div class="col-6 p-3">
          <h2 class="text-light fw-bold">Start Learning to Drive Today</h2>
          <p class="text-light fw-bold">Give us a call to schedule your first driving lesson</p>
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
  </main>
</template>

<script>
import Form from "./MainComponents/Form.vue";

export default {
  components: {
    Form,
  },
};
</script>

<style lang="scss">
.learn-to-drive-today {
  background-image: url("../assets/siteAssets/horizontal-cta-background.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}
</style>