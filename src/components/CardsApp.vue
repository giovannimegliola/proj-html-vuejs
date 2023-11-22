<template>
  <div class="container">
    <div class="row">
      <div class="col-md-4" v-for="card in cards" :key="card.id">
        <div class="card">
          <img :src="card.image" class="card-img-top" alt="Card image"> 
          <div class="card-body">
            <p class="card-price">{{ card.price }}</p>
            <h5 class="card-title">{{ card.title }}</h5>
            <p class="card-text">{{ card.info }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import { cards } from '../data/cards';
  export default {
    name: 'CardsApp',
    data(){
      return{
        cards,
      }
    }
  }
</script>

<style lang="scss" scoped>

.card{
  margin-bottom: 40px;
  border: none;
  cursor: pointer;
  overflow: hidden;
}

.card img{
  transition: transform .8s ease;
}
.card:hover{
  box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.5);
}
.card:hover img {
  transform: scale(1.1);
}
.card-price{
  color: #20ad96;
  font-weight: 600;
  font-size: 20px;
}

.card-title{
  color: #3f3a64;
  margin-bottom: 20px;
}

.card-title:hover{
  color: #20ad96;
  cursor: pointer;
}
.card-text{
  color: #696969 ;
  font-size: 13px;
  font-weight: 300;
}

</style>