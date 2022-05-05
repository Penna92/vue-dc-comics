<template>
  <div id="jumbotron"></div>
</template>

<script>
export default {
  name: "AppJumbotron",
  // props: {
  //   msg: String
  // }
  data() {
    return {};
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/variables.scss";
@import "../style/general.scss";
#jumbotron {
  width: 100%;
  height: 50vh;
  background: url(../assets/img/jumbotron.jpg);
  background-size: cover;
}
</style>
