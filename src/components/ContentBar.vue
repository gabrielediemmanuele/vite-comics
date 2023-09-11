<script>
//* Import component ComicCard and comicsList from data/comics.js array.
import ComicCard from "./ComicCard.vue";
import comicsList from "../data/comics";
export default {
  data() {
    return {
      // array comicsList
      comicsList,
    };
  },
  // props call from ComicCard component
  components: {
    ComicCard,
  },
};
</script>

<template>
  <div class="jumbotron"></div>
  <div class="content-bar">
    <button class="button-series">CURRENT SERIES</button>
    <div class="comics-cont">
      <!--*  Component ComicCard  -->
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
  position: relative;

  .button-series {
    width: 150px;
    margin-bottom: 20px;
    background-color: #0282f9;
    color: white;
    border: none;
    padding: 10px;
    position: absolute;
    top: -14px;
    left: 213px;
    font-weight: bolder;
    &:hover {
      background-color: #ffffff;
      color: #0282f9;
      transition: 1s;
    }
  }
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
