<script>
export default {
  data() {
    return {};
  },
};
</script>

<template>
  <div class="container">
    <img src="../../public/img/dc-logo.png" alt="" />
  </div>
</template>

<style lang="scss" scoped>
@use "../styles/general.scss" as *;

.container {
  @include cont_settings();
  background-color: white;
}
</style>
