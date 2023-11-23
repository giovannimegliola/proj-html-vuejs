<template>
  <section id="stories">
    <div class="row">
      <div class="col-md-6 text-center">
        <h4 class="py-3">REAL STORIES</h4>
        <div class="carousel">
          <p class="mytext py-3 ">{{ currentStory.text }}</p>
          <img :src="currentStory.image" :alt="currentStory.name"/>
          <p class="py-2 myname">{{ currentStory.name }} </p> 
          <p class="myrole">{{ currentStory.role }}</p>
        </div>
        <button @click="prevSlide" class="mybtn"> &#60; </button>
        <button @click="nextSlide" class="mybtn"> &#62;</button>
      </div>
      <div class="col-md-6">
        <img src="../assets/images/home-movation-testimonial-image-768x562.jpg" alt=""/>
      </div>
    </div>
  </section>
</template>

<script>
import {stories} from "../data/stories.js"
export default {
  name: "StoriesApp",
  data() {
    return {
      stories,
      currentSlide: 0,
    };
  },  
  computed: {
    currentStory(){
      return this.stories[this.currentSlide];
    },
  },
  methods: {
    prevSlide() {
      this.currentSlide = (this.currentSlide - 1 + this.stories.length) % this.stories.length;
    },
    nextSlide() {
      this.currentSlide = (this.currentSlide + 1) % this.stories.length;
    },
  },
};
</script>

<style lang="scss" scoped>
#stories {
  background-image: url(../assets/images/background-pattern-wavify.png);
}

h4 {
  color: #20ad96;
}

.carousel {
  position: relative;
  width: 100%;
  max-width: 400px; 
  margin: 0 auto; 
}

.carousel img {
  width: 90px;
  height: auto;
  border-radius: 50%;
}

button {
  margin: 10px;
}

.mytext{
  font-size: 27px;
  font-weight: 200;
}

.myname{
  font-size: 20px;
}

.myrole{
  font-size: 15px;
  font-weight: 200;
}

.mybtn{
  border-radius: 50%;
  border: none;
}
</style>
