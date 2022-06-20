<template>
  <div class="bg_foot">
    <div class="button_container">


      <button class="foot_button">
        <a href="#">
          <img src="../assets/svg/svg-3.svg" alt="">
          Purchase Theme
        </a>
      </button>


      <button class="foot_button">
        <a href="#">
          <img src="../assets/svg/svg-2.svg" alt="">
          Related Theme
        </a>
      </button>

    </div>

    <div class="social_container">
      <a href="#"><img src="../assets/img/theme_eduprime_logo.png" alt=""></a>
      <p>EduPrime is the most versatile WordPress theme for educational purposes, showcasing universities, courses,
        secondary school etc.</p>
      <a href="#">
        <font-awesome-icon class="brand_icon facebook_icon" icon="fa-brands fa-facebook-f" />
      </a>
      <a href="#">
        <font-awesome-icon class="brand_icon" icon="fa-brands fa-twitter" />
      </a>
      <a href="#">
        <font-awesome-icon class="brand_icon" icon="fa-brands fa-instagram" />
      </a>

    </div>

    <div class="links_container">
      <div class="link_foot">
        <h3>Get EduPrime</h3>
        <ul>
          <li v-for="(item, i) in linksFoot" :key="i">
            <a :href="item.url">
              {{ item.text }}
            </a>
          </li>
        </ul>
      </div>

      <div class="link_foot">
        <h3>Networking</h3>
        <ul>
          <li v-for="(itemLink, j) in linksFootNet" :key="j">
            <a :href="itemLink.url">
              {{ itemLink.text }}
            </a>
          </li>
        </ul>
      </div>
    </div>

    <div class="search_container">
      <div class="search_bar">
        <input type="text" placeholder="Search...">
        <font-awesome-icon class="icon_search" icon="fa-solid fa-magnifying-glass" />
        <h4>Search categories</h4>
      </div>
      <div class="buttons_container">

        <button class="empty_button">
          <a href="#">ECONOMY</a>
        </button>

        <button class="empty_button">
          <a href="#">DESIGN</a>
        </button>

        <button class="empty_button">
          <a href="#">COACHING</a>
        </button>

        <button class="empty_button">
          <a href="#">BUSINESS</a>
        </button>

        <button class="empty_button">
          <a href="#">MEDICINE</a>
        </button>

        <button class="empty_button">
          <a href="#">LAW</a>
        </button>

        <button class="empty_button">
          <a href="#">FITNESS</a>
        </button>

      </div>

      <p>ModelTheme.All rights reserved.</p>
    </div>

    <div class="bact_top">
      <a href="#">
        <img src="../assets/img/back-to-top-arrow.svg" alt="">
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'EPFooter',
  data() {
    return {
      linksFoot: [
        {
          text: "Request a website",
          url: "#"
        },
        {
          text: "Browse Themes",
          url: "#",
        },
        {
          text: "Paymant options",
          url: "#",
        },
        {
          text: "Support System",
          url: "#",
        },
        {
          text: "Chechout",
          url: "#",
        },
        {
          text: "Purchase Theme",
          url: "#",
        }
      ],

      linksFootNet: [
        {
          text: "Purchase Theme",
          url: "#"
        },
        {
          text: "Our Benefits",
          url: "#",
        },
        {
          text: "Our Team",
          url: "#",
        },
        {
          text: "Our Services",
          url: "#",
        },
        {
          text: "Other Products",
          url: "#",
        },
        {
          text: "My account",
          url: "#",
        }
      ]
    }
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/button.scss';

$primary_pink: #E56768;

// links style
a {
  text-decoration: none;
  color: #ffffffCC;
}

ul li {
  list-style: none;
  margin: 10px 0;
}

.bg_foot {
  height: 400px;
  background-color: $primary_pink;
  display: flex;
  padding-top: 100px;
  color: #ffffffCC;

  .button_container {
    padding-left: 30px;
    padding-top: 170px;
  }

  .foot_button {
    background-color: #454545;
    border: none;
    border-radius: 5px;
    width: 170px;
    height: 30px;
    margin: 10px 0;
    box-shadow: 0 5px 10px rgba($color: #000000, $alpha: 0.6);
  }

  .foot_button a {
    display: flex;
    align-items: center;
    color: #8b8b8a;
    padding: 5px 10px;
    font-size: 12px;



    img {
      width: 15px;
      margin: 0 5px;
    }
  }

  .social_container {
    width: 40%;
    font-size: 15px;

    img {
      width: 250px;
    }

    p {
      margin: 25px 0;
    }
  }

  .brand_icon {
    font-size: 15px;
    margin-right: 10px;
    border: 2px solid #E9D758;
    padding: 10px;
    border-radius: 50%;
  }

  .facebook_icon {
    padding-left: 13px;
    padding-right: 13px;
  }

  .links_container {
    display: flex;
    width: 50%;
  }

  .link_foot {
    color: white;
    padding-left: 30px;
    width: 50%;

    h3 {
      margin-bottom: 25px;
      font-size: 20px;
    }
  }

  .search_container {
    padding-right: 10px;
    text-align: right;

    .search_bar {
      position: relative;
    }

    input {
      padding: 20px 10px;
      padding-right: 150px;
      border: none;
      border-radius: 25px;
    }

    .icon_search {
      color: white;
      padding: 20px;
      background-color: #E9D758;
      border-radius: 50%;
      position: absolute;
      top: 0;
      right: -5px;
    }

    h4 {
      color: white;
      margin: 10px 0;
      margin-top: 20px;
    }

    p {
      color: #E9D758;
      margin: 40px 0;
      font-size: 15px;
    }
  }

  .bact_top {
    display: flex;
    align-items: flex-end;
    justify-content: flex-end;
    width: 10%;
    img {
      background-color: #E9D758;
      padding: 8px;
      border-radius: 50%;
      margin: 10px 20px;
    }
  }

  .buttons_container {
    display: flex;
    justify-content: flex-end;
    flex-wrap: wrap;
  }
}
</style>