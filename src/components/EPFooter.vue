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

    </div>

    <div class="links_container">

    </div>

    <div class="search_container">

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
      ]
    }
  },

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
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
$primary_pink: #E56768;

.bg_foot {
  height: 400px;
  background-color: $primary_pink;

  .button_container {
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    padding-left: 30px;
    padding-top: 270px;
    width: 15%;
  }

  .foot_button{
    background-color: #454545;
    border: none;
    border-radius: 5px;
    width: 170px;
    height: 30px;
    margin: 10px 0;
    box-shadow: 0 5px 10px rgba($color: #000000, $alpha: 0.6);
  }
  .foot_button a{
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
}
</style>