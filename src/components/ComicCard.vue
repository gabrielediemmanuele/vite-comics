<script>
export default {
  data() {
    return {};
  },
  props: {
    comic: Object,
  },
};
</script>

<template>
  <div class="card">
    <img :src="comic.thumb" alt="" />
    <h6>{{ comic.series }}</h6>
    <span class="price">{{ comic.price }}</span>
    <span class="type">{{ comic.type }}</span>
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: 120px;
  height: 200px;
  margin: 8px 8px 8px 8px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  &:hover {
    background-color: #0282f9;
    transform: scale(1.2);
    transition: 500ms;
    padding: 8px;
    border-radius: 5px;
  }

  img {
    width: 100%;
    height: 120px;
    object-fit: cover;
  }
  h6 {
    margin: 4px 0 8px 0;
    color: white;
  }
  &:hover .price {
    color: white;
  }
  &:hover .type {
    color: white;
  }

  span {
    color: white;
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
