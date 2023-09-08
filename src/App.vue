<script>
import Header_nav from "./components/Header_nav.vue";
import Content_bar from "./components/Content_bar.vue";
import Products_bar from "./components/Products_bar.vue";
import Footer_Links from "./ccomponents/Footer_Links.vue";
import Footer_socials from "./ccomponents/Footer_socials.vue";

export default {
  components: {
    Header_nav,
    Content_bar,
    Products_bar,
    Footer_Links,
    Footer_socials,
  },
};
</script>

<template>
  <h1>titolo</h1>
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
</style>
