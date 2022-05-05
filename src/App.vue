<template>
  <div id="app">
    <AppHeader />
    <main>
      <AppJumbotron />
      <AppGrid />
    </main>
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import AppJumbotron from "./components/AppJumbotron.vue";
import AppGrid from "./components/AppGrid.vue";
export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
    AppJumbotron,
    AppGrid,
  },
};
</script>

<style lang="scss">
@import "./style/variables.scss";
@import "./style/general.scss";
#app {
  min-width: 1000px;
  background-color: rgb(28, 28, 28);
}
main {
  margin-top: 100px;
  background-color: rgb(28, 28, 28);
  width: 100%;
}
</style>
