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
            <h5>{{ item.text }}</h5>
          </div>

        </div>

        <div class="carousel_content">
          <div class="img_content">
            <img src="../assets/img/Gavel-Illustration-e1556884768193.png" alt="">
          </div>

          <div class="text_content">
            <h2>
              Law Faculty
            </h2>

            <p>
              Learning from world-leading academics and practitioners, you'll not only receive an outstanding grounding
              in the theory of law, but you will be able to understand how those principles are applied in practice
              through a range of student-led activities and competitions.
            </p>

            <button class="btn_pink">
              Read More
            </button>
          </div>
        </div>
      </div>
    </section>

    <div class="wawe">
      <img src="../assets/svg/svg-0.svg" alt="">
    </div>

    <section class="time_line_container">

      <div class="time_line">
        <div class="title_time_line">
          <img src="../assets/img/Clock-and-Bell.png" alt="">
          <br>
          <h2>University Year</h2>
        </div>

        <div class="time_line_content">

          <div class="time_line_flex">
            <div class="text_time_line">
              <h4>Demo Classes</h4>
              <p>In the first students try to accomodate with the teaching style and choose their optional courses.</p>
            </div>

            <div class="text_time_line">
              <h4>Graduation Day</h4>
              <p>On the day of graduation, all students gather for the ceremony and then network and party among others.
              </p>
            </div>
          </div>

          <img src="../assets/img/Timeline-Item.png" alt="">

          <div class="time_line_flex2">
            <div class="text_time_line2">
              <h4>Orientation</h4>
              <p>First day of the universuty year, all students gather for the opening ceremony and then network with others.</p>
            </div>

            <div class="text_time_line2">
              <h4>Evaluation</h4>
              <p>At the end of a semester, students take a general evaluation test for every subject they're learning.
              </p>
            </div>
          </div>

        </div>
      </div>
    </section>

    <section class="events_container">
      <img src="../assets/img/upcoming-events-calendar-icon.png" alt="">
      <h2>Upcoming Events</h2>
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

// first section style
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

// carousel container style
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
    width: 70%;
    margin: 20px auto;
  }

  .img_carousel {
    padding: 40px 60px;
    color: #E56768;
    border: 1px solid #ECECEE;
    cursor: pointer;
    box-shadow: 0 10px 5px #dedede;

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

  .carousel_content {
    width: 70%;
    margin: 30px auto;
    display: flex;
    text-align: left;

    .img_content {
      width: 50%;
    }

    .text_content {
      width: 50%;

      p {
        color: #8b8b8a;
        margin: 20px 0;
      }
    }
  }

}

.wawe {
  overflow: hidden;

  img {
    width: 180%;
    display: block;
  }
}

.time_line_container {
  color: white;

  .time_line {
    background-color: #E56768;
    text-align: center;
    padding-top: 20px;

    img {
      width: 50px;
      margin: 10px;
    }

    h2 {
      display: inline;
      background-color: #DB2A2C;
      font-size: 40px;
    }
  }

  .time_line_content {

    h4{
      font-size: 20px;
      font-weight: 900;
      margin: 10px 0;
    }

    img {
      width: 1000px;
    }

    .time_line_flex {
      display: flex;
      justify-content: center;

      .text_time_line {
        width: 25%;
        margin-top: 50px;
        margin-left: 100px;
      }
    }

    .time_line_flex2 {
      display: flex;
      margin-left: 300px;

      .text_time_line2 {
        width: 25%;
        margin-right: 100px;
      }
    }
  }
}

.events_container{
  background-color: #E56768;
  text-align: center;
  padding-top: 50px;
  color: white;

  img{
    width: 50px;
  }
  
  h2{
    font-size: 50px;
    font-weight: 900;
  }
}
</style>