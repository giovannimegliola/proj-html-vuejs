<template>
  <div class="text-center">
    <p class="myp">BEGIN YOUR JOURNEY AT MAXCOACH</p> 
    <h2><span style="color: #3f3a64;">Latest</span> Online Courses</h2>
  </div>
  <CardsApp />
  <div class="text-center">
    <a href="#" class="btn mybtn">View all courses  &#8594;</a>
  </div>
</template>

<script>
  import CardsApp from './CardsApp.vue';
  export default {
    name: 'CoursesApp', 
    components: {
      CardsApp
    }
  }
</script>

<style lang="scss" scoped>
h2{
  font-size: 50px;
  color: #20ad96;
  margin-bottom: 50px;
}

.mybtn{
  background-color: #20ad96;
  padding: 15px 40px;
  margin-top: 20px;
  color: white;
}
.mybtn:hover{
  background-color: #3f3a64;
}

.myp{
  margin-top: 70px ;
}

</style>