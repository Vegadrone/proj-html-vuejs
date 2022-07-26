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
      <div class="col-9">
        <coursesCard />
      </div>
    </div>
  </div>
</template>

<script>
import coursesCard from "./coursesCard.vue"

    export default {

        data: function(){
            return{
                coursesCardVoices: [
                    {
                        serviceName: 'Pass Plus',
                        imgPath: '../../assets/siteAssets/courses-passplus-200x200.jpg',
                        btn: 'learn more',
                    },
                    {
                        serviceName: 'Intensive Course',
                        imgPath: '../../assets/siteAssets/course-intensive-200x200.jpg',
                        btn: 'learn more',
                    },
                    {
                        serviceName: 'Instructors',
                        imgPath: '../../assets/siteAssets/courses-instructor-200x200.jpg',
                        btn: 'learn more',
                    },
                ]
            }
        },

        component:{
            coursesCard,
        }

    };
</script>

<style lang="scss">
.course-card {
  border: 2px solid black;

  button {
    display: block;
    margin: 0 auto;
  }
}
</style>