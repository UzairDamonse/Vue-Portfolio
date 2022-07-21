<template>
  <Navbar />
  <router-view />
</template>

<script>
import Navbar from "./components/Navbar.vue";
export default {
  components: {
    Navbar,
  },
};
</script>

<style>
* {
  font-family: elder;
  user-select: none;
  cursor: url("../src/assets/Skyrim-normal.cur"), auto;
}
@font-face {
  font-family: skyrim;
  src: url("../src/assets/darks-skyrim-font/DarkXShadowSkyrim.ttf");
}

@font-face {
  font-family: elder;
  src: url(@/assets/planewalker/Planewalker.ttf);
}

:root {
  --white: #cdd1c8;
  --black: #303030;
  --grey: #bfbfbf;
  --blue: #316e7b;
  --red: #ed254e;
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
