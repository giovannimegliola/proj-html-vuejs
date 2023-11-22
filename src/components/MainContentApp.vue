<template>
    <HeroApp />
    <section id="about">
      About me
    </section>
    <section id="courses">
      Online courses
    </section>
    <section id="books">
      Book store
    </section>
    <section id="stories">
     Real stories
    </section>
    <section id="blog">
      Blog Updates
    </section>
</template>

<script>
  import HeroApp from './HeroApp.vue';
  export default {
    name: 'MainContentApp',
    components:{
      HeroApp
    }
    
  }
</script>

<style lang="scss" scoped>

</style>