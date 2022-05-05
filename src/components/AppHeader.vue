<template>
  <header>
    <div>
      <img src="../assets/img/dc-logo.png" alt="DC Logo" />
    </div>
    <ul>
      <li v-for="(item, index) in links" :key="index">
        <a :class="{ selected: item.active }" href="#">{{ item.testo }}</a>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  // props: {
  //   msg: String
  // }
  data() {
    return {
      links: [
        {
          testo: "Characters",
          link: "",
          active: false,
        },
        {
          testo: "Comics",
          link: "",
          active: true,
        },
        {
          testo: "Movies",
          link: "",
          active: false,
        },
        {
          testo: "Tv",
          link: "",
          active: false,
        },
        {
          testo: "Games",
          link: "",
          active: false,
        },
        {
          testo: "Collectibles",
          link: "",
          active: false,
        },
        {
          testo: "Videos",
          link: "",
          active: false,
        },
        {
          testo: "Fans",
          link: "",
          active: false,
        },
        {
          testo: "News",
          link: "",
          active: false,
        },
        {
          testo: "Shop",
          link: "",
          active: false,
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../style/variables.scss";
@import "../style/general.scss";

.selected {
  color: $azzurro;
  border-bottom: 5px solid $azzurro;
}

header {
  height: 100px;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  padding: 0 10%;
  background-color: white;
  display: flex;
  align-items: center;
  justify-content: space-between;
  z-index: 9999;
  // min-width: 1000px;
  overflow-x: auto;
  overflow-y: hidden;
  div {
    margin-left: 40px;
    img {
      vertical-align: middle;
      height: 70px;
      width: 70px;
    }
  }
  ul {
    margin-right: 40px;
    height: 100%;
    display: flex;
    line-height: 100px;
    gap: 10px;
    li {
      display: flex;
      align-items: center;
      height: 100%;
      list-style-type: none;
      a {
        height: 100%;
        text-decoration: none;
        color: black;
        text-transform: uppercase;
        font-weight: bold;
      }
    }
  }
}
</style>
