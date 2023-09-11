<script>
export default {
  data() {
    return {};
  },
};
</script>

<template>
  <div class="jumbotron"></div>
  <div class="content-bar">
    <div class="comics-cont">bla bla</div>
  </div>
</template>

<style lang="scss" scoped>
.jumbotron {
  width: 100%;
  height: 200px;
  background-image: url(../../public/img/jumbotron.jpg);
  background-size: cover;
}
.content-bar {
  width: 100%;
  background-color: #1c1c1c;
}
.comics-cont {
  width: 70%;
  height: 50px;
  margin: 0 auto;
  padding: 20px;
  display: flex;
  align-items: center;
  span {
    font-size: 25px;
    color: white;
  }
}
</style>
