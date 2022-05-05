<template>
  <div id="upper-footer">
    <ul>
      <li v-for="(item, index) in links" :key="index">
        <img :src="item.icon" :alt="item.description" />
        <a href="#">{{ item.description }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "AppUpperFooter",
  // props: {
  //   msg: String
  // }
  data() {
    return {
      links: [
        {
          icon: require("../assets/img/buy-comics-digital-comics.png"),
          description: "Digital Comics",
          link: "",
          active: false,
        },
        {
          icon: require("../assets/img/buy-comics-merchandise.png"),
          description: "DC Merchandise",
          link: "",
          active: false,
        },
        {
          icon: require("../assets/img/buy-comics-subscriptions.png"),
          description: "Subscription",
          link: "",
          active: false,
        },
        {
          icon: require("../assets/img/buy-comics-shop-locator.png"),
          description: "Comic Shop locator",
          link: "",
          active: false,
        },
        {
          icon: require("../assets/img/buy-dc-power-visa.svg"),
          description: "DC Power Visa",
          link: "",
          active: false,
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import "../style/variables.scss";
#upper-footer {
  position: absolute;
  top: 0;
  width: 100%;
  height: 150px;
  background-color: $azzurro;
  z-index: 9999;
  ul {
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 30px;
    li {
      color: white;
      height: 30%;
      list-style-type: none;
      display: flex;
      align-items: center;
      gap: 10px;
      cursor: pointer;
      img {
        height: 100%;
      }
      a {
        text-decoration: none;
        color: white;
      }
    }
  }
}
</style>