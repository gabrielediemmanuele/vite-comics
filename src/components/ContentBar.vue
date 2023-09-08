<script>
export default {
  data() {
    return {};
  },
};
</script>

<template>
  <div class="content-bar">
    <div class="container">
      <span> &rarr; Content goes here... &larr;</span>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.content-bar {
  width: 100%;
  background-color: #1c1c1c;
}
.container {
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
