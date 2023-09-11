<script>
import comicsList from "../data/comics";

export default {
  data() {
    return {
      comicsList,
    };
  },
  props: {
    comic: Array,
  },
};
</script>

<template>
  <div class="card">
    <img :src="comicsList.thumb" alt="" />
    <h5>{{ comicsList.series }}</h5>
    <span class="price">{{ comicsList.price }}</span>
    <span class="type">{{ comicsList.type }}</span>
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: 120px;
  margin: 5px 5px 5px 5px;
  border: 1px solid red;
  display: flex;
  flex-direction: column;

  img {
    width: 100%;
    height: 120px;
    object-fit: cover;
  }
  h5 {
    margin: 2px 0 2px 0;
    color: white;
  }
  span {
    color: white;
    margin: 2px 0 2px 0;
  }
  .price {
    font-size: 20px;
    color: #0282f9;
  }
  .type {
    font-size: 10px;
    color: #929292;
  }
}
</style>
