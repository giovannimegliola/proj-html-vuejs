<template>
    <HeroApp />
    <AboutMeApp />
    <CoursesApp />
    <BooksApp />
    <StoriesApp />
    <BlogApp />
</template>

<script>
  import HeroApp from './HeroApp.vue';
  import AboutMeApp from './AboutMeApp.vue';
  import CoursesApp from './CoursesApp.vue';
  import BooksApp from './BooksApp.vue';
  import StoriesApp from './StoriesApp.vue';
  import BlogApp from './BlogApp.vue';
  export default {
    name: 'MainContentApp',
    components:{
      HeroApp,
      AboutMeApp,
      CoursesApp,
      BooksApp,
      StoriesApp,
      BlogApp
    } 
  }
</script>

<style lang="scss" scoped>

</style>