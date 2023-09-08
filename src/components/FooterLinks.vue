<script>
export default {
  data() {
    return {
      DcComics: [
        "Characters",
        "Comics",
        "Movies",
        "TV",
        "Games",
        "Videos",
        "News",
      ],

      DcLinks: [
        "Terms of Use",
        "Privacy police (New)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],

      SitesLinks: [
        "DC",
        "MAD Magazine",
        "DC Kids",
        "DC Universe",
        "DC Power Visa",
      ],

      ShopLinks: ["Shop DC", "Shop DC Collectibles"],
    };
  },
};
</script>

<template>
  <div class="footer-links-cont">
    <div class="container">
      <div class="gen-links-cont">
        <div class="link-col">
          <h4>DC COMICS</h4>
          <span v-for="dccomic in DcComics">{{ dccomic }}</span>
          <h4>SHOP</h4>
          <span v-for="shoplink in ShopLinks">{{ shoplink }}</span>
        </div>
        <div class="link-col">
          <h4>DC</h4>
          <span v-for="dclink in DcLinks">{{ dclink }}</span>
        </div>
        <div class="link-col">
          <h4>SITES</h4>
          <span v-for="sitelink in SitesLinks">{{ sitelink }}</span>
        </div>
      </div>
      <div class="logo-cont"></div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.footer-links-cont {
  width: 100%;
  height: 280px;
  background-image: url(../../public/img/footer-bg.jpg);
}
.container {
  width: 70%;
  height: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  /* border: 1px solid red; */
  .gen-links-cont {
    width: 50%;
    height: 80%;
    /* border: 1px solid green; */
    margin: auto 0;
    display: flex;
    align-items: center;
    justify-content: center;
    .link-col {
      width: calc(100% / 3);
      height: 80%;
      /* border: 1px solid rgb(176, 156, 156); */
      display: flex;
      flex-direction: column;
      margin: 0 10px;
      h4 {
        margin: 3px 0;
        color: white;
        font-size: 13px;
      }
      span {
        font-size: 8px;
        color: rgb(184, 184, 184);
        margin: 2px 0;
      }
    }
  }
}
.logo-cont {
  width: 50%;
  height: 100%;
  /* border: 1px solid green; */
  margin: auto 0;
  background-image: url(../../public/img/dc-logo-bg.png);
  background-size: cover;
  background-position: center;
}
</style>
