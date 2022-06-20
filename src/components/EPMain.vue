<template>
  <main>
    <section class="first_section_bg">
      <div class="container_70">
        <div class="col_left">
          <img class="book_icon" src="../assets/img/Books-icon.png" alt="">
          <h2>Thousand of courses for any type of student</h2>
          <p>At EduPrime, it doesn't matter what domain you wish to pursue a career in. Here you can find a courses that
            satisfies your needs within a click away and applies for a course in a matter of minutes. EduPrime is ranked
            as the most versatile university in the world, thanks to the number of courses it provides.</p>
          <button class="btn_yellow">
            <a href="#">
              browse through courses
            </a>
          </button>
        </div>

        <div class="col_right">
          <img src="../assets/img/Graduation-Illustration.png" alt="">
        </div>
      </div>
    </section>

    <section class="carousel_container">
      <h2>Faculties avaible at EduPrime</h2>
      <div class="text_carousel">
        <p>A single university with a load of courses, tailored to satisfy any student's needs.</p>
      </div>

      <div class="carousel">
        <div class="nav_carousel">

          <div v-for="(item, i) in carousel" :key="i" class="img_carousel" :class="item.current ? 'active' : ''">
          <img :src="item.urlImg" alt="">
          <h5>{{item.text}}</h5>
          </div>

        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: 'EPMain',
  data() {
        return {
            carousel: [
                {
                    text: "Law faculty",
                    urlImg: require("../assets/img/Gavel-v2.png"),
                    current: true
                },
                {
                    text: "Economy",
                    urlImg: require("../assets/img/Coins-tabs-v2.png"),
                    current: false
                },
                {
                    text: "Medicine",
                    urlImg: require("../assets/img/Medicine-tabs-v2.png"),
                    current: false
                },
                {
                    text: "Computer Science",
                    urlImg: require("../assets/img/Computer-tabs-v2.png"),
                    current: false
                },
                {
                    text: "Graphic Design",
                    urlImg: require("../assets/img/Palette-tabs-v2.png"),
                    current: false
                }
            ]
        }
    }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/button.scss';

$primary_text: #3D404F;

.first_section_bg {
  background-image: url(../assets/img/home-background.png);
  background-size: cover;
  background-repeat: no-repeat;

  .container_70 {
    width: 70%;
    margin: 0 auto;
    display: flex;
    padding: 40px 0;

    .book_icon {
      width: 40px;
    }
  }

  .col_left {
    width: 50%;
    color: $primary_text;

    h2 {
      font-weight: 900;
      font-size: 40px;
      margin: 20px 0;
    }

    button {
      margin-top: 20px;
    }
  }

  .col_right {
    width: 50%;
    margin-left: 50px;

    img {
      width: 600px;
    }
  }
}

.carousel_container {

  text-align: center;

  h2 {
    color: $primary_text;
    font-size: 40px;
    font-weight: 900;
  }

  .text_carousel {
    width: 25%;
    margin: 30px auto;

    p {
      color: $primary_text;
    }
  }

  .nav_carousel {
    display: flex;
  }

  .img_carousel {
    padding: 40px 60px;
    color: #E56768;
    border: 1px solid #ECECEE;

    img {
      width: 100px;
    }
  }

  // active item carousel
  .active {
    background-color: #E56768;
    color: white;
    border: none;

    img {
      filter: brightness(500%);
    }

  }

}
</style>