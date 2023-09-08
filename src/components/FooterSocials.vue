<script>
export default {
  data() {
    return {
      socials: [
        "../../public/img/footer-facebook.png",
        "../../public/img/footer-periscope.png",
        "../../public/img/footer-pinterest.png",
        "../../public/img/footer-twitter.png",
        "../../public/img/footer-youtube.png",
      ],
    };
  },
};
</script>

<template>
  <footer>
    <div class="container">
      <button>SING-UP NOW!</button>
      <div class="socials-cont">
        <span> FOLLOW US </span>
        <span v-for="social in socials">
          <img :src="social" :alt="social" />
        </span>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
  width: 100%;
  background-color: #303030;
}
.container {
  width: 70%;
  height: 80px;
  margin: 0 auto;
  background-color: #303030;
  display: flex;
  justify-content: space-between;
  align-items: center;

  button {
    border: 3px solid #0282f9;
    padding: 10px;
    background-color: transparent;
    color: #ffffff;
  }

  button:hover {
    border: 3px solid #ffffff;
    padding: 10px;
    background-color: #ffffff;
    color: #0282f9;
    transition: 1s;
  }

  .socials-cont {
    display: flex;
    align-items: center;

    img {
      width: 20px;
    }

    span {
      margin: 0 8px;
      color: #0282f9;
      font-weight: bold;
      font-style: italic;
    }
  }
}
</style>
