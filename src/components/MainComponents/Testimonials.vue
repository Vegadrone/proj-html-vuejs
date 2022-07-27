<template>
  <div>
    <h2 class="fw-bold text-center">Testimonials</h2>
    <p class="text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque eligendi veritatis at quidem eum!</p>
    <Slide v-for="(slide, index) in testimonialSlideElements" :key="index"
    :img="slide.img"
    :text="slide.text"
    :name="slide.name"/>
  </div>
</template>

<script>
import Slide from "./Slide.vue";

export default {

    components:{
        Slide
    },

  data: function () {
    return {
      testimonialSlideElements: [
        {
          img: "testimonial-sophia.png",
          text: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quaerat ratione libero, repellendus nemo ea doloremque architecto pariatur, commodi explicabo officiis, vero doloribus aspernatur. Nisi saepe, in sunt soluta commodi provident!",
          name: "Sophia Jones",
        },
        // {
        //   img: "testimonial-grant.png",
        //   text: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quaerat ratione libero, repellendus nemo ea doloremque architecto pariatur, commodi explicabo officiis, vero doloribus aspernatur. Nisi saepe, in sunt soluta commodi provident!",
        //   name: "Grant Barret",
        // },
        // {
        //   img: "testimonial-harold.png",
        //   text: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quaerat ratione libero, repellendus nemo ea doloremque architecto pariatur, commodi explicabo officiis, vero doloribus aspernatur. Nisi saepe, in sunt soluta commodi provident!",
        //   name: "Harold Hammer",
        // },
        // {
        //   img: "testimonial-kate.png",
        //   text: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quaerat ratione libero, repellendus nemo ea doloremque architecto pariatur, commodi explicabo officiis, vero doloribus aspernatur. Nisi saepe, in sunt soluta commodi provident!",
        //   name: "Kate Bishop",
        // },
        // {
        //   img: "testimonial-kelly.png",
        //   text: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quaerat ratione libero, repellendus nemo ea doloremque architecto pariatur, commodi explicabo officiis, vero doloribus aspernatur. Nisi saepe, in sunt soluta commodi provident!",
        //   name: "Kelly Brewster",
        // },
      ],
    };
  },
};
</script>

<style>
</style>