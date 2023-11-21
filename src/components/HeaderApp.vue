<template>
  <header class="bg-white py-4">
    <div class="container">
      <div class="row">
        <div class="col-md-3">
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
        <div class="col-md-3">
            <i class="fa-brands fa-twitter mx-3"></i>
            <i class="fa-brands fa-facebook-f mx-3"></i>
            <i class="fa-brands fa-instagram mx-3"></i>
            <i class="fa-brands fa-linkedin mx-3"></i>
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
.logo{
  width: 160px;
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