<template>
  <header class="bg-white py-4">
    <div class="container">
      <div class="row">
        <div class="col-md-3">
          <a href="#" >
            <img src="../assets/images/dark-logo.png" alt="MaxCoach logo" class="logo" />
          </a>
        </div>
        <div class="col-md-7">
          <nav class="d-flex justify-content-between align-items-center">
            <ul class="nav">
              <li v-for="(link,index) in links" :key="index" class="nav-item">
                <a v-bind:href="link.href" class="nav-link" :class="{ active: link.active }" @mouseover="toggleDropdown(index)" @mouseleave="link.showDropdown = false">
                  {{ link.text }} <i class="fa-solid fa-angle-down myicon"></i>
                </a>
                <div v-if="link.showDropdown" class="dropdown-content">
                  <ul>
                    <li>MaxCoach education</li>
                    <li>Course Portal</li>
                    <li>Modern Schooling</li>
                    <li>Health Coaching</li>
                    <li>Business</li>
                    <li>Courses Grid</li>
                  </ul>
                </div>
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
    },
    methods: {
    toggleDropdown(index) {
      // Nascondi tutti i dropdown
      this.links.forEach((link) => {
        link.showDropdown = false;
      });

      // Mostra il dropdown del link cliccato
      this.links[index].showDropdown = true;
    },
  },
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
.myicon{
  font-size: 10px;
}
.dropdown-content {
  display: block;
  position: absolute;
  background-color: #f9f9f9;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  z-index: 1;
}
.dropdown-content ul {
  list-style: none;
  padding: 0;
  margin: 0;
}
.dropdown-content li {
  padding: 10px;
  text-align: left;
}
</style>