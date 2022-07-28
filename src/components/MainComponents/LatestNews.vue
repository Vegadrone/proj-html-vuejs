<template>
  <div class="container">
    <div class="row d-flex justify-content-center">
        <div class="col-10">
            <h2 class="fw-bold text-center">Latest News</h2>
        </div>
        <div class="col-10">
 
        </div>
    </div>
  </div>
</template>

<script>


export default {
    name: "LatestNews",
    component:{
       
    },

    data: function(){
        return{
            newsElements:[
                {
                    img:"blog-choosecar-700x441.jpg",
                    title:"What Car to Start With?",
                    date:"February 7th 2019",
                    comments:"3 comments",
                    text:"Lorem ipsum sit dolor amet, consectetur adipiscing"
                },
                 {
                    img:"blogpost-10and2-700x441.jpg",
                    title:"Avada Driving School Expanding",
                    date:"February 27th 2019",
                    comments:"7 comments",
                    text:"Lorem ipsum sit dolor amet, consectetur adipiscing"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
  .col-10{
    background-color: #fff;
  }
</style>