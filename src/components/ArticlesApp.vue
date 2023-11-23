<template>
  <div class="row">
    <div class="col-md-3" v-for="article in articles" :key="article.id">
      <div class="card">
        <img :src="article.image" class="article-img-top" alt="article image" />
        <div class="article-body py-4 ">
          <p class="article-date">{{ article.date }}</p>
          <h5 class="article-title">{{ article.title }}</h5>
          <p class="article-text">{{ article.text }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { articles } from "../data/articles";
export default {
  name: "ArticlesApp",
  data() {
    return {
      articles,
    };
  },
};
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
.card:hover img {
  transform: scale(1.1);
}

.article-title:hover{
  color: #20ad96;
}

.article-text{
  font-size: 14px;
}

.article-date{
  font-size: 14px;
}
</style>
