<!--* Array for Navigation Menù -->
<script>
export default {
  data() {
    return {
      navlist: [
        "CHARACTERS",
        "COMICS",
        "MOVIES",
        "TV",
        "GAMES",
        "COLLECTIBLES",
        "VIDEOS",
        "FANS",
        "NEWS",
        "SHOP",
      ],
    };
  },
};
</script>

<template>
  <header>
    <div class="container">
      <img src="../../public/img/dc-logo.png" alt="" />
      <ul>
        <!--* For Cicle to generate the navlist from the array  -->
        <li v-for="list in navlist">{{ list }}</li>
      </ul>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use "../styles/general.scss" as *;

header {
  width: 100%;
  background-color: $head_bg_color;
}
.container {
  width: 70%;
  margin: 0 auto;
  padding: 10px;
  background-color: $head_bg_color;
  display: flex;

  ul {
    margin: 0;
    padding: 0;
    display: flex;
    list-style-type: none;
    align-items: center;
    margin-left: auto;
    font-size: 10px;

    li {
      margin-left: 10px;
      margin-right: 10px;
      font-weight: bold;
    }

    li:hover {
      color: #0282f9;
      text-underline-offset: 28px;
      text-decoration: underline;
      text-decoration-color: #0282f9;
      text-decoration-thickness: 3px;
    }
  }

  img {
    width: 50px;
  }
}
</style>
