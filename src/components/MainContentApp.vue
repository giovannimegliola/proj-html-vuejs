<template>
    <HeroApp />
    <AboutMeApp />
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
  import AboutMeApp from './AboutMeApp.vue';
  export default {
    name: 'MainContentApp',
    components:{
      HeroApp,
      AboutMeApp
    }
    
  }
</script>

<style lang="scss" scoped>

</style>