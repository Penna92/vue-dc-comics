<template>
  <div id="app">
    <!-- <h1>Benvenuto</h1>
    <p>Daje</p> -->
    <AppHeader />
    <AppFooter />
    <header></header>
    <main></main>
    <footer></footer>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
  },
};
</script>

<style lang="scss">
@import "./style/variables.scss";
@import "./style/general.scss";
main {
  background-color: black;
  width: 100%;
  position: absolute;
  top: 100px;
  bottom: 100px;
  height: calc(100vh - 200px);
}
</style>
