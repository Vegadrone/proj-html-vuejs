<template>
  <div class="container">
    <div class="row">
      <div class="col-3">
        <div class="course-card">
          <img
            src="../../assets/siteAssets/new-corner.jpg"
            alt="new-corner.jpg"
          />
          <h3 class="text-center fw-bold">Courses</h3>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Eligendi
            ipsa quaerat voluptas sit incidunt aspernatur. Voluptas
            reprehenderit sapiente nesciunt quaerat repellendus possimus
            officiis voluptatum, dignissimos vitae commodi aut beatae at!
          </p>
          <button class="btn btn-success text-light text-uppercase">
            courses information
          </button>
        </div>
      </div>
      <div class="col-9 d-flex justify-content-around">
        <ServiceCard
          v-for="(card, index) in serviceCardEl"
          :key="index"
          :imgPath="card.imgPath"
          :serviceName="card.serviceName"
          :buttonText="card.btn"
        />
      </div>
    </div>
  </div>
</template>

<script>
import ServiceCard from "./ServiceCard.vue";

export default {

    components:{
        ServiceCard
    },

    data: function () {
    return {
      serviceCardEl: [
        {
          serviceName: "Pass Plus",
          imgPath: "courses-passplus-200x200.jpg",
          btn: "learn more",
        },
        {
          serviceName: "Intensive Course",
          imgPath: "course-intensive-200x200.jpg",
          btn: "learn more",
        },
        {
          serviceName: "Instructors",
          imgPath: "courses-instructor-200x200.jpg",
          btn: "learn more",
        },
      ],
    };
  },
}
</script>

<style lang="scss">
  .course-card {
    border: 2px solid black;
  }

</style>