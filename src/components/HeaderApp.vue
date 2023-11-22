<template>
  <header class="bg-white py-4">
    <div class="container">
      <div class="row">
        <div class="col-md-4">
          <a href="#" >
            <img src="../assets/images/dark-logo.png" alt="MaxCoach logo" class="logo" />
          </a>
        </div>
        <div class="col-md-6">
          <nav class="d-flex justify-content-between align-items-center">
            <ul class="nav">
              <li v-for="(link,index) in links" :key="index" class="nav-item">
                <a v-bind:href="link.href" class="nav-link" :class="{ active: link.active }">
                  {{ link.text }}
                </a>
              </li>
            </ul>
          </nav>
        </div>
        <div class="col-md-2">
            <i class="fa-brands fa-twitter ms-4 "></i>
            <i class="fa-brands fa-facebook-f ms-4"></i>
            <i class="fa-brands fa-instagram ms-4"></i>
            <i class="fa-brands fa-linkedin ms-4"></i>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
  import { links } from '../data/links';
  export default {
    name: 'HeaderApp',
    data(){
      return{
        links
      };
    }
  }
</script>

<style lang="scss" scoped>
header{
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000;
}
.logo{
  width: 150px;
}
.nav-link {
  color: #3f3a64;
}
.nav-link:hover {
  color: #20ad96;
}
i{
  font-size: 20px;
  cursor: pointer;
}
i:hover{
  color: #20ad96;
}
</style>