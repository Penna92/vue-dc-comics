<template>
  <footer>
    <AppUpperFooter />
    <div id="central-footer">
      <div id="center-left-footer">
        <ul>
          <li><h2>DC COMICS</h2></li>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>
          <li><h2>SHOP</h2></li>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
        </ul>
        <ul>
          <li><h2>DC</h2></li>
          <li><a href="#">Terms Of Use</a></li>
          <li><a href="#">Privacy Policy (Nes)</a></li>
          <li><a href="#">Ad Choices</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Talent Workshops</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>

        <ul>
          <li><h2>SITES</h2></li>
          <li><a href="#">DC</a></li>
          <li><a href="#">MAD Magazine </a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>
      </div>
      <div id="center-right-footer">
        <img src="../assets/img/dc-logo-bg.png" alt="DC Logo Background" />
      </div>
    </div>
    <div id="bottom-footer">
      <div id="bottom-left-footer">
        <button>SIGN-UP NOW!</button>
      </div>
      <div id="bottom-right-footer">
        <h4>FOLLOW US</h4>
        <ul>
          <li v-for="(item, index) in social" :key="index">
            <a href="#">
              <img :src="item.icon" :alt="'Icona' + item.icon" />
            </a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
import AppUpperFooter from "./AppUpperFooter.vue";
export default {
  name: "AppFooter",
  components: {
    AppUpperFooter,
  },
  // props: {
  //   msg: String
  // }
  data() {
    return {
      social: [
        {
          icon: require("../assets/img/footer-facebook.png"),
          link: "",
          active: false,
        },
        {
          icon: require("../assets/img/footer-twitter.png"),
          link: "",
          active: true,
        },
        {
          icon: require("../assets/img/footer-youtube.png"),
          link: "",
          active: false,
        },
        {
          icon: require("../assets/img/footer-pinterest.png"),
          link: "",
          active: false,
        },
        {
          icon: require("../assets/img/footer-periscope.png"),
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
footer {
  // width: 80%;
  // min-width: 1000px;
  position: relative;
  // height: 50vh;
  #central-footer {
    overflow-y: auto;
    // z-index: 1;
    // width: 80%;
    background: url(../assets/img/footer-bg.jpg) center center no-repeat;
    background-size: cover;
    display: flex;
    align-items: center;
    justify-content: space-between;
    // position: fixed;
    // height: 50vh;
    // bottom: 100px;
    #center-left-footer {
      display: flex;
      margin-top: 40px;
      margin-bottom: 40px;
      margin-left: 10%;
      h2 {
        color: white;
      }
      ul {
        margin-top: 50px;
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        gap: 10px;
        margin-right: 20px;
        li {
          list-style-type: none;
          a {
            text-decoration: none;
            color: $grey-font;
            &:hover {
              color: white;
              font-weight: bold;
            }
          }
        }
      }
    }
    #center-right-footer {
      margin-top: 40px;
      margin-bottom: 40px;
      margin-right: 10%;
    }
  }
  #bottom-footer {
    background-color: $bg-dark-grey;
    width: 100%;
    height: 100px;
    z-index: 999;
    position: absolute;
    bottom: 0;
    // position: fixed;
    // bottom: 0;
    // left: 0;
    display: flex;
    align-items: center;
    justify-content: space-between;
    #bottom-left-footer {
      margin-left: 10%;
      button {
        padding: 10px;
        color: white;
        border: 1px solid $azzurro;
        background-color: $bg-dark-grey;
        cursor: pointer;
        &:hover {
          background-color: $hover;
        }
      }
    }
    #bottom-right-footer {
      display: flex;
      align-items: center;
      h4 {
        color: $azzurro;
        margin-right: 10px;
      }
      ul {
        display: flex;
        gap: 10px;
        li {
          // overflow: hidden;
          padding: auto;
          line-height: 30px;
          height: 30px;
          width: 30px;
          border-radius: 50%;
          list-style-type: none;
          text-align: center;
          &:hover {
            background-color: white;
            // overflow: hidden;
          }
          a {
            text-decoration: none;
            color: $bg-dark-grey;
          }
        }
      }
      margin-right: 10%;
    }
  }
}
</style>