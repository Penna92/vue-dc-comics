<template>
  <div id="app">
    <!-- <h1>Benvenuto</h1>
    <p>Daje</p> -->
    <AppHeader />
    <main>
      <AppJumbotron />
    </main>
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import AppJumbotron from "./components/AppJumbotron.vue";
export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
    AppJumbotron,
  },
};
</script>

<style lang="scss">
@import "./style/variables.scss";
@import "./style/general.scss";
#app {
  min-width: 1000px;
}
main {
  margin-top: 100px;
  background-color: yellow;
  width: 100%;
}
</style>
