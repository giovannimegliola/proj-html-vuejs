<template>
  <footer class="py-4">
    <div class="container">
      <div class="row">
        <div class="col-md-6">
          <h5>Address</h5>
          <ul class="list-unstyled">
            <li v-for="(item,index) in lists.address" :key="index" class="py-2">{{ item }}</li>
          </ul>
          <i class="fa-brands fa-square-facebook"></i>
          <i class="fa-brands fa-twitter ms-4"></i>
          <i class="fa-brands fa-instagram ms-4"></i>
          <i class="fa-brands fa-linkedin ms-4"></i>
        </div>
        <div class="col-md-4">
          <h5>Explore</h5>
          <ul class="list-unstyled">
            <li v-for="(item,index) in lists.explore" :key="index" class="py-2">{{ item }}</li>
          </ul>
        </div>
        <div class="col-md-2">
          <h5>Information</h5>
          <ul class="list-unstyled">
            <li v-for="(item,index) in lists.information" :key="index" class="py-2">{{ item }}</li>
          </ul>
        </div>
      </div> 
      <p class="text-center py-4 ">&#169; 2020 Maxcoach. All Rights Reserved</p>
    </div>
  </footer>
</template>


<script>
  import { lists } from '../data/lists.js'
  export default {
    name: 'FooterApp',
    data(){
      return{
        lists,
      }
    } 
  }
</script>

<style lang="scss" scoped>
footer{
  background-color:#181621 ;
  color: #696969 ;
  font-size: 0.9em;
}

h5{
  color: white;
}

i{
  font-size: 20px;
  cursor: pointer;
}

i:hover{
  color: white;
}

li{
  cursor: pointer;
}
li:hover{
  color: #20ad96;
}
</style>