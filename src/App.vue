<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  name: "App",
  components: { AppHeader, AppMain, AppFooter }
}
</script>

<template>
  <app-header></app-header>
  <app-main></app-main>
  <app-footer></app-footer>
</template>

<style>
/* reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* generics */
body {
  font-family: "Open Sans", sans-serif;
  min-height: 100vh;
}

img {
  max-width: 100%;
  height: auto;
}

li {
  list-style-type: none;
}

a {
  text-decoration: none;
  font-weight: bold;
  padding: 20px 10px;
}

/* utils */
.container {
  max-width: 1140px;
  margin: 0 auto;
}
</style>