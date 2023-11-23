<template>
    <HeroApp />
    <AboutMeApp />
    <CoursesApp />
    <BooksApp />
    <StoriesApp />
    <section id="blog">
      Blog Updates
    </section>
</template>

<script>
  import HeroApp from './HeroApp.vue';
  import AboutMeApp from './AboutMeApp.vue';
  import CoursesApp from './CoursesApp.vue';
  import BooksApp from './BooksApp.vue';
  import StoriesApp from './StoriesApp.vue';
  export default {
    name: 'MainContentApp',
    components:{
      HeroApp,
      AboutMeApp,
      CoursesApp,
      BooksApp,
      StoriesApp 
    } 
  }
</script>

<style lang="scss" scoped>

</style>