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
              <p>First day of the universuty year, all students gather for the opening ceremony and then network with
                others.</p>
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

      <div class="card_container">
        <div class="my_card">
          <h3>Coaching Sessions</h3>
          <h6>
            <font-awesome-icon icon="fa-solid fa-calendar-days" /> 20 May 21:30 PM
          </h6>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores, corrupti! [...]</p>
          <button class="btn_pink_little">
            <font-awesome-icon icon="fa-solid fa-plus" /> Find More
          </button>
        </div>

        <div class="my_card">
          <h3>Coaching Sessions</h3>
          <h6>
            <font-awesome-icon icon="fa-solid fa-calendar-days" /> 24 Ma3 18:00 PM
          </h6>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores, corrupti! [...]</p>
          <button class="btn_pink_little">
            <font-awesome-icon icon="fa-solid fa-plus" /> Find More
          </button>
        </div>

        <div class="my_card">
          <h3>Coaching Sessions</h3>
          <h6>
            <font-awesome-icon icon="fa-solid fa-calendar-days" /> 12 Feb 13:30 PM
          </h6>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores, corrupti! [...]</p>
          <button class="btn_pink_little">
            <font-awesome-icon icon="fa-solid fa-plus" /> Find More
          </button>
        </div>
      </div>

      <span><button class="btn_yellow">View All Events</button></span>

    </section>

    <section class="latest_courses_container">
      <div class="wawe_container">
        <img src="../assets/svg/svg-1.svg" alt="">
      </div>



      <div class="courses_card_container">
        <h2>Latest Courses</h2>
        <div class="courses_card">
          <img src="../assets/img/Decisions-icon.png" alt="">
          <h3>Make Better Decisions</h3>
          <h5>
            <font-awesome-icon icon="fa-regular fa-user" /> Teacher: <b>James Colins</b>
          </h5>
          <h5>
            <font-awesome-icon icon="fa-solid fa-money-bill-1" /> Price: <b>€21.00</b>
          </h5>
          <button class="btn_pink_little">
            <font-awesome-icon icon="fa-regular fa-eye" /> View Course
          </button>
        </div>

        <div class="courses_card">
          <img src="../assets/img/Speaker-icon.png" alt="">
          <h3>How to be a speacker</h3>
          <h5>
            <font-awesome-icon icon="fa-regular fa-user" /> Teacher: <b>James Colins</b>
          </h5>
          <h5>
            <font-awesome-icon icon="fa-solid fa-money-bill-1" /> Price: <b>Free</b>
          </h5>
          <button class="btn_pink_little">
            <font-awesome-icon icon="fa-regular fa-eye" /> View Course
          </button>
        </div>

        <div class="courses_card">
          <img src="../assets/img/Network-icon.png" alt="">
          <h3>Network Introductions</h3>
          <h5>
            <font-awesome-icon icon="fa-regular fa-user" /> Teacher: <b>James Colins</b>
          </h5>
          <h5>
            <font-awesome-icon icon="fa-solid fa-money-bill-1" /> Price: <b>Free</b>
          </h5>
          <button class="btn_pink_little">
            <font-awesome-icon icon="fa-regular fa-eye" /> View Course
          </button>
        </div>

        <div class="courses_card">
          <img src="../assets/img/Brand-icon.png" alt="">
          <h3>Brand Management</h3>
          <h5>
            <font-awesome-icon icon="fa-regular fa-user" /> Teacher: <b>James Colins</b>
          </h5>
          <h5>
            <font-awesome-icon icon="fa-solid fa-money-bill-1" /> Price: <b>Free</b>
          </h5>
          <button class="btn_pink_little">
            <font-awesome-icon icon="fa-regular fa-eye" /> View Course
          </button>
        </div>
      </div>

    </section>

    <section class="info_container">
      <div class="col_text_info">
        <img src="../assets/img/Exam-icon.png" alt="">
        <h2>The Most Efficient examination method</h2>
        <p>EduPrime has gathered teachers from around the globe to brainstorm in order to facilitate the evaluation of
          our students. Every teacher from our university has an influence on how students are evalutaded at his/her
          subject.</p>
        <button class="btn_pink">Discover the Method</button>
      </div>

      <div class="col_img_info">
        <img src="../assets/img/Exam-Illustration.png" alt="">
      </div>

      <div class="col_img_info">
        <img src="../assets/img/Girl-Illustration.png" alt="">
      </div>

      <div class="col_text_info">
        <img src="../assets/img/Exam-icon-1.png" alt="">
        <h2>Variable fees for international students</h2>
        <p>EduPrime has gathered teachers from around the globe to brainstorm in order to facilitate the evaluation of
          our students. Every teacher from our university has an influence on how students are evalutaded at his/her
          subject.</p>
        <button class="btn_pink">List of Fees</button>
      </div>

    </section>

    <section class="sub_bg">
      <div class="sub_container">
        <div class="title_sub">
          <h2>Subscribe Now to Our Newsletter !</h2>
        </div>

        <div class="search_sub">
          <div class="search_bar">
            <input type="text" placeholder="Search...">
            <font-awesome-icon class="icon_search" icon="fa-solid fa-magnifying-glass" />
          </div>
        </div>
      </div>
    </section>

    <section class="partners_container">
      <div class="text">
        <h2>Partners</h2>
        <p>Leverage agile framework to provide a robust synopsis for high level overviews. Iterative approaches to
          corporate strategy.</p>
      </div>

      <div class="img_partners_container">
        <a href="#"><img class="big_img" src="../assets/img/partner-1.png" alt=""></a>
        <a href="#"><img class="little_img" src="../assets/img/partner-2.png" alt=""></a>
        <a href="#"><img class="big_img" src="../assets/img/partner-3.png" alt=""></a>
        <a href="#"><img class="big_img" src="../assets/img/partner-4.png" alt=""></a>
        <a href="#"><img class="little_img" src="../assets/img/partner-5.png" alt=""></a>
        <a href="#"><img class="big_img" src="../assets/img/partner-6.png" alt=""></a>
        <a href="#"><img class="little_img" src="../assets/img/partner-7.png" alt=""></a>
      </div>

      <div class="wawe_bg">
        <img src="../assets/img/background-wave3.png" alt="">
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

.btn_yellow {
  margin: 30px 0;
}

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

    &:hover {
      background-color: #E56768;
      color: white;
      border: none;

      img {
        filter: brightness(500%);
      }
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

    h4 {
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

.events_container {
  background-color: #E56768;
  text-align: center;
  padding-top: 50px;
  color: white;

  img {
    width: 50px;
  }

  h2 {
    font-size: 50px;
    font-weight: 900;
  }
}

.card_container {
  display: flex;
  justify-content: space-evenly;
  width: 70%;
  margin: 0 auto;

  .my_card {
    width: 300px;
    background-color: white;
    color: #8b8b8a;
    padding: 20px;
    border-radius: 10px;
    height: 170px;
    margin: 50px 0;

    h3 {
      color: #3D404F;
      font-weight: 900;
    }

    h6 {
      margin: 5px;
    }

    .btn_pink_little {
      box-shadow: 5px 10px 40px #000000CC;
      margin-top: 20px;
    }
  }



}

.wawe_container {
  overflow: hidden;

  img {
    width: 150%;
    display: block;
    margin-left: -15px;
    margin-top: -1px;
  }
}

.latest_courses_container {
  background-color: white;

  h2 {
    font-weight: 900;
    color: #3D404F;
    font-size: 40px;
    width: 100%;
  }

  .courses_card_container {
    width: 70%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;

    .courses_card {
      text-align: center;
      width: 220px;
      height: 200px;
      color: #8b8b8a;
      border: 1px solid #ECECEE;
      box-shadow: 5px 5px 5px #dedede;
      margin: 40px 0;

      h3 {
        color: #3D404F;
        font-weight: 900;
      }

      h5 {
        margin: 10px;
      }

      b {
        color: #3D404F;
      }

      img {
        width: 70px;
        margin: 10px 0;
      }
    }
  }
}

.info_container {
  width: 80%;
  margin: 0 auto;
  margin-top: 40px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;

  .col_text_info {
    width: 40%;
    margin: 20px 0;

    h2 {
      font-weight: 900;
      font-size: 40px;
      color: #3D404F;
      margin-top: 10px;
    }

    img {
      width: 70px;
    }

    p {
      color: #3D404F;
      margin: 30px 0;
    }
  }

  .col_img_info {
    width: 50%;
    margin: 20px 0;

    img {
      width: 500px;
    }
  }
}

.sub_bg {
  background-color: #E56768;

  .sub_container {
    width: 80%;
    margin: 0 auto;
    display: flex;
    justify-content: space-evenly;
    padding: 30px 0;

    .title_sub {
      color: white;

      h2 {
        font-weight: 900;
      }
    }

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
      // position: absolute;
      // top: 0;
      // right: -5px;
      margin: -22px -45px;
    }
  }
}

.partners_container {

  .text {
    width: 30%;
    margin: 20px auto;
    text-align: center;

    h2 {
      color: #3D404F;
      font-weight: 900;
      font-size: 30px;
    }

    p {
      color: #3D404F;
      margin: 20px 0;
    }
  }

  .img_partners_container {
    width: 70%;
    margin: 30px auto;

    .big_img {
      width: 70px;
    }

    .little_img {
      width: 180px;
    }

    img {
      margin: 0 10px;
      filter: opacity(40%);
    }

    a img:hover {
      filter: none;
    }

  }

  .wawe_bg {
    background-color: #F7F8FA;

    img {
      width: 100%;
      height: 200px;
    }
  }
}
</style>