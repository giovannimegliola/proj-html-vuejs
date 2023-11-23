<template>
  <div class="container mtop">
    <h4>BLOG UPDATED</h4>
    <p class="myp">Interesting <span style="color: #20ad96;">articles updated</span> daily</p>
    <ArticlesApp/>
    <p class="myp1">VIEW ALL POSTS</p>
  </div>
</template>

<script>
  import ArticlesApp from './ArticlesApp.vue';
  export default {
    name:'BlogApp',
    components: {
      ArticlesApp
    }
  }
</script>

<style lang="scss" scoped>
.myp{
  font-size: 40px;
  margin-bottom: 50px;
}

.myp1{
  color: #20ad96;
  text-align: center;
  cursor: pointer;
  margin-bottom: 100px;
}
.myp1:hover{
  color: #3f3a64;
}

.mtop{
  margin-top: 90px;
}
</style>