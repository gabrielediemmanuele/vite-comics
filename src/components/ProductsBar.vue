<script>
export default {
  data() {
    return {
      products: [
        {
          image: "../../public/img/buy-comics-digital-comics.png",
          title: "DIGITAL COMICS",
        },
        {
          image: "../../public/img/buy-comics-merchandise.png",
          title: "DC MERCHANDISE",
        },
        {
          image: "../../public/img/buy-comics-subscriptions.png",
          title: "SUBSCRIPTION",
        },
        {
          image: "../../public/img/buy-comics-shop-locator.png",
          title: "COMIC SHOP LOCATOR",
        },
        {
          image: "../../public/img/buy-dc-power-visa.svg",
          title: "DC POWER VISA",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="products-bar">
    <div class="container">
      <div class="img-cont" v-for="product in products">
        <img :src="product.image" :alt="product.title" />
        <span> {{ product.title }}</span>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.products-bar {
  width: 100%;
  background-color: #0282f9;
}
.container {
  width: 70%;
  height: 50px;
  margin: 0 auto;
  padding: 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  .img-cont {
    display: flex;
    font-size: 12px;
    color: white;
    align-items: center;
    margin-left: 10px;
    margin-right: 10px;
    img {
      width: 30px;
      height: 35px;
      margin-right: 5px;
    }
  }
}
</style>
