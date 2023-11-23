<template>
  <section id="about">
    <div class="container">
      <h4>ABOUT ME</h4>
      <div class="row">
        <div class="col-md-4">
          <p class="myp">How to Be an Alpha Male: The 15 Habits of True Alphas</p>
        </div>
        <div class="col-md-6 ms-auto">
          <strong><p>Want to learn how to be an alpha male? How to be more masculine? How to be the man you’ve always wanted to be?</p></strong>
          <p>Your goal is to show the consistency of business, core values, and customer care. Punctuality, responsibility, individuality, accuracy, enthusiasm - you have to clearly explain how these qualities are applicable to your work. And the important thing is you do love what you do.</p>
        </div>
        <div class="row">
          <div class="col-md-7 py-5">
            <div class="backimg">
              <img src="../assets/images/home-movation-video-poster-670x450.jpg" alt="video youtube" class="myimg">        
              <img src="../assets/images/icon-youtube-play.png" alt="icona youtube" class="img-overlay" >
            </div>
          </div>
          <div class="col-md-5 py-5">
            <p class="myp2">"Every morning you have two choices: continue to sleep with your dreams, or wake up and chase them."</p>
            <img src="../assets/images/home-movation-shape-01.png" alt="shape" class="py-4">
            <strong><p>Kaixa Stark</p></strong>
            <p>WINGMAN</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name:'AboutMeApp'
  }
</script>

<style lang="scss" scoped>

h4{
  color: #20ad96;
  font-size: 20px;
  margin-top: 70px;
  margin-bottom: 30px;
}

.backimg{
  position: relative;
  display: block;
  margin-right: 40px ;
}

.backimg img{
  cursor: pointer;
}

.img-overlay{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: block;
}
.myp{
  font-size: 35px;
  font-weight: 400;
}

img{
  border-radius: 7px;
}

.myimg{
  width: 100%;
}
.myp2{
  font-size: 25px;
  margin-top: 60px;
  font-weight: 300;
}


.backimg{
  overflow: hidden;
}
.myimg{
  transition: transform .8s ease;
}

.myimg:hover {
  transform: scale(1.1);
}
</style>