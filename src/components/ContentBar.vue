<script>
import ComicsCard from "./ComicsCard.vue";
export default {
  data() {
    return {
      ComicsCard,
    };
  },
};
</script>

<template>
  <div class="jumbotron"></div>
  <div class="content-bar">
    <div class="label-series"></div>
    <div class="comics-cont">
      <ComicsCard
        v-for="(comic, index) in comicsList"
        :key="index"
        :comic="comic"
      ></ComicsCard>
    </div>
    <button class="load-more-button"></button>
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
}
.comics-cont {
  width: 70%;
  margin: 0 auto;
  padding: 20px;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}
</style>
