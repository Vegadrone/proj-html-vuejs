<template>
  <div class="form-wrapper">
    <form>
        <h3 class="mt-3 text-center">First Lesson Free!</h3>
        <p class=" mt-4 text-center">When you make a block booking with us your first lesson is included free.</p>
        <input class="mt-3 mb-2" type="text" :placeholder="formValue" v-for="(formValue, index) in formValues" :key="index">
        <button class="btn btn-success text-uppercase">request a callback</button>
    </form>
  </div>
</template>

<script>
export default {
    data: function(){
        return{
            formValues:[
                'Your Name*',
                'Email*',
                'Telephone*',
                'Location*'
            ]
        }
    }
};
</script>

<style lang="scss">
    .form-wrapper{
        border: 2px solid black;

        input,
        button{
            display: block;
            margin: 0 auto;
        }

    }
</style>