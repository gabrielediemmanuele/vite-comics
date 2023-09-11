<script>
import HeaderNav from "./components/HeaderNav.vue";
import ContentBar from "./components/ContentBar.vue";
import ProductsBar from "./components/ProductsBar.vue";
import FooterLinks from "./components/FooterLinks.vue";
import FooterSocials from "./components/FooterSocials.vue";

export default {
  data() {
    return {};
  },

  components: {
    HeaderNav,
    ContentBar,
    ProductsBar,
    FooterLinks,
    FooterSocials,
  },
};
</script>

<template>
  <HeaderNav></HeaderNav>
  <ContentBar></ContentBar>
  <ProductsBar></ProductsBar>
  <FooterLinks></FooterLinks>
  <FooterSocials></FooterSocials>
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
</style>
