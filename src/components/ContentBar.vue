<script>
import ComicCard from "./ComicCard.vue";
import comicsList from "../data/comics";
export default {
  data() {
    return {
      comicsList,
    };
  },
  components: {
    ComicCard,
  },
};
</script>

<template>
  <div class="jumbotron"></div>
  <div class="content-bar">
    <div class="label-series"></div>
    <div class="comics-cont">
      <ComicCard
        v-for="(comic, index) in comicsList"
        :key="index"
        :comic="comic"
      ></ComicCard>
    </div>
    <button class="load-button">LOAD MORE</button>
  </div>
</template>

<style lang="scss" scoped>
.jumbotron {
  width: 100%;
  height: 250px;
  background-image: url(../../public/img/jumbotron.jpg);
  background-size: cover;
}
.content-bar {
  width: 100%;
  background-color: #1c1c1c;
  display: flex;
  flex-direction: column;
  align-items: center;
  .load-button {
    width: 150px;
    margin-bottom: 20px;
    background-color: #0282f9;
    color: white;
    border: none;
    padding: 10px;
    &:hover {
      background-color: #ffffff;
      color: #0282f9;
      transition: 1s;
    }
  }
}
.comics-cont {
  width: 70%;
  margin: 20px auto;
  padding: 20px;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  justify-content: center;
}
</style>
