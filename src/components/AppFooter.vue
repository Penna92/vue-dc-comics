<template>
  <footer></footer>
</template>

<script>
export default {
  name: "AppFooter",
  // props: {
  //   msg: String
  // }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/variables.scss";
footer {
  background-color: $bg-dark-grey;
  width: 100%;
  height: 100px;
  position: fixed;
  bottom: 0;
  left: 0;
}
</style>