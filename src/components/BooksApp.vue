<template>
  <div class="container py-5 ">
    <div class="row">
      <div class="col-md-4">
        <h5 class="py-3">BOOK STORE ONLINE</h5>
        <p class="myp1">Be Alpha With</p>
        <p class="myp2">Wingman's Book</p>
        <ul class="list-unstyled">
          <li><i class="fa-solid fa-check myicon"></i>Help you understand yourself better</li>
          <li><i class="fa-solid fa-check myicon"></i>Revealing mature tips</li>
          <li><i class="fa-solid fa-check myicon"></i>Give the right advice</li>
          <li><i class="fa-solid fa-check myicon"></i>Fascinating examples of alpha man</li>
        </ul>
        <a href="#" class="btn mybtn">Get free ebook</a>
      </div>
      <div class="col-md-4" v-for="book in books" :key="book.id">
        <div class="card">
          <img :src="book.image" class="card-img-top" alt="Book image"> 
          <div class="card-body text-center">
            <h5 class="book-title">{{ book.title }}</h5>
            <p class="book-price">{{ book.price }}</p>
          </div>
        </div>
      </div>
    </div>
    <div class="row py-5">
      <div class="col-md-2">
        <a href="#"><img src="public/images/client-logo-05-primary.png" alt="It's Alive logo"></a>
      </div>
      <div class="col-md-2">
        <a href="#"><img src="public/images/client-logo-06-primary.png" alt="It's Alive logo"></a>
      </div>
      <div class="col-md-2">
        <a href="#"><img src="public/images/client-logo-07-primary.png" alt="It's Alive logo"></a>
      </div>
      <div class="col-md-2">
        <a href="#"><img src="public/images/client-logo-04-primary.png" alt="It's Alive logo"></a>
      </div>
      <div class="col-md-2 ">
        <a href="#"><img src="public/images/client-logo-03-primary.png" alt="It's Alive logo"></a>
      </div>
      <div class="col-md-2">
        <a href="#"><img src="public/images/client-logo-02-primary.png" alt="It's Alive logo"></a>
      </div>
    </div>

  </div>
</template>

<script>
  import { books } from '../data/books.js'
  export default {
    name:'BooksApp',
    data(){
      return{
        books,
      }
    }
  }
</script>

<style lang="scss" scoped>

.myp1{
  color: #3f3a64;
  font-size: 40px;
  margin-bottom: 5px;
}
.myp2{
  color: #20ad96;
  font-size: 40px ;
}
.myicon{
  color: #20ad96;
  margin-right: 10px;
  margin-top: 15px;
}

.mybtn{
  background-color: #20ad96;
  padding: 15px 40px;
  margin-top: 20px;
  color: white;
}
.mybtn:hover{
  background-color: #3f3a64;
}

.book-price{
  color: #20ad96;
  font-weight: 600;
  font-size: 20px;
}

.book-title{
  color: #3f3a64;
  margin-bottom: 20px;
}
</style>