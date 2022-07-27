<template>
  <div class="container">
    <div class="row">
      <div class="col-8">
        <h2 class="fw-bold">Your Instructors</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aperiam
          consectetur magnam sequi amet nemo odit odio, expedita ut sunt enim,
          perferendis nisi eos doloremque accusamus ad nesciunt natus unde
          culpa!
        </p>
      </div>
      <div class="col-4">
        <button class="btn btn-success text-uppercase">more about us</button>
      </div>
    </div>
    <div class="row">
      <div class="col-4 d-flex text-center">
        <SquareCard
          v-for="(instructorCardEl, index) in instructorsCardsElements"
          :key="index"
          :img="instructorCardEl.img"
          :name="instructorCardEl.name"
          :text="instructorCardEl.text"
        />
      </div>
    </div>
  </div>
</template>

<script>
import SquareCard from "./SquareCard.vue";
export default {
  name:"Insctructors",
  components: {
    SquareCard,
  },

  data: function () {
    return {
      instructorsCardsElements: [
        {
          img: "instructor-mikehart-400x254.jpg",
          name: "Mike Hart",
          text: "Lorem ipsum dolor sit amet, consecutur adipiscing elit",
        },
        {
          img: "instructor-johnsmith-400x254.jpg",
          name: "John Smith",
          text: "Lorem ipsum dolor sit amet, consecutur adipiscing elit",
        },
        {
          img: "instructor-angelahart-400x254.jpg",
          name: "Angela Hart",
          text: "Lorem ipsum dolor sit amet, consecutur adipiscing elit",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
</style>