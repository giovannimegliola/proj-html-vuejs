<template>
  <HeaderApp /> Header
  <MainContentApp /> Main Content
  <FooterApp />Footer
</template>

<script>
  import HeaderApp from './components/HeaderApp.vue';
  import MainContentApp from './components/MainContentApp.vue';
  import FooterApp from './components/FooterApp.vue';
  export default {
    name: 'App',
    components: {
      HeaderApp,
      MainContentApp,
      FooterApp
    }
  }
</script>

<style lang="scss" scoped>

</style>