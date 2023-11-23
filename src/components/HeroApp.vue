<template>
  <section id="hero">
  <div class="container py-5">
    <div class="row">
      <div class="col-md-6 py-5 ">
        <p>I'M WINGMAN</p>
        <h1>Peace On Earth A Wonderful Wish But No Way</h1>
        <p>Success isn’t overnight. It’s when everyday you get a little</p>
        <p>better than the day before. It all adds up.</p>
        <a href="#" class="btn mybtn">Get started for free  &#8594;</a>
      </div>
      <div class="col-md-6">
        <img src="../assets/images/home-movation-hero-image.png" alt="Max Coach image">
      </div>
    </div>   
  </div>
  </section>
  <section id="stats">
    <div class="container">
      <div class="row text-center py-5">
      <div class="col-md-3">
        <div>
          <h3>1.926</h3>
          <p>FINISHED SESSIONS</p>
        </div>
      </div>
      <div class="col-md-3">
        <div>
          <h3>100%</h3>
          <p>SATISFACTION RATE</p>
        </div>
      </div>
      <div class="col-md-3">
        <div>
          <h3>3092+</h3>
          <p>ENROLLED LEARNERS</p>
        </div>
      </div>
      <div class="col-md-3">
        <div>
          <h3>200</h3>
          <p>ONLINE INSTRUCTORS</p>
        </div>
      </div>    
    </div> 
    </div>
  </section>
</template>

<script>
  export default {
    name: 'HeroApp'
  }
</script>

<style lang="scss" scoped>
#hero{
  background-image: url('../assets/images/background-pattern-wavify.png');
  margin-top: 100px;
}

h1{
  font-size: 65px;
  margin-bottom: 20px;
}

h3{
  color: #20ad96;
  font-size: 35px;
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
</style>