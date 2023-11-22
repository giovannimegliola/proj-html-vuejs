<template>
    <HeroApp />
    <AboutMeApp />
    <CoursesApp />
    <BooksApp />
    
    <section id="stories">
      Real stories
    </section>
    <section id="blog">
      Blog Updates
    </section>
</template>

<script>
  import HeroApp from './HeroApp.vue';
  import AboutMeApp from './AboutMeApp.vue';
  import CoursesApp from './CoursesApp.vue';
  import BooksApp from './BooksApp.vue';
  export default {
    name: 'MainContentApp',
    components:{
      HeroApp,
      AboutMeApp,
      CoursesApp,
      BooksApp 
    } 
  }
</script>

<style lang="scss" scoped>

</style>