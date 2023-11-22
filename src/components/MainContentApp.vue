<template>
    <HeroApp />
    <AboutMeApp />
    <CoursesApp />
    
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
  import AboutMeApp from './AboutMeApp.vue';
  import CoursesApp from './CoursesApp.vue';
  export default {
    name: 'MainContentApp',
    components:{
      HeroApp,
      AboutMeApp,
      CoursesApp
      
    }
    
  }
</script>

<style lang="scss" scoped>

</style>