<template>
    <header>
        <div class="header_jumbo_container">
            <div class="bg_color">
                <!-- header e navbar -->
                <div class="container_header">
                    <a href="#"><img src="../assets/img/theme_eduprime_logo.png" alt="logo"></a>
                    <nav>
                        <ul>
                            <li v-for="(link, i) in links" :key="i">
                                <a :href="link.url" :class="link.current ? 'active' : ''"
                                    @click="link.current = !link.current">
                                    {{ link.text }}
                                    <font-awesome-icon class="icon_down" icon="fa-solid fa-caret-down" />
                                </a>
                            </li>
                        </ul>
                        <button class="btn_yellow">
                            VIEW COURSES
                        </button>
                    </nav>
                </div>

                <!-- Jumbotron -->
                <div class="container_jumbo">
                    <h2 class="title_jumbo">
                        Key to your succes
                    </h2>

                    <p>EduPrime is the most versatile WordPress theme for educational purposes, showcasting
                        universities, courses, secondary school etc.</p>

                    <div class="btn_container">
                        <button class="btn_yellow">
                            <font-awesome-icon icon="fa-solid fa-magnifying-glass" /> Search courses
                        </button>

                        <button class="btn_white">
                            <font-awesome-icon icon="fa-solid fa-user-plus" /> Apply for university
                        </button>
                    </div>
                </div>

            </div>

        </div>

        <div class="wave_container">
            <img src="../assets/img/Wave-1.png" alt="">
        </div>
    </header>
</template>

<script>
export default {
    name: 'EPHeader',
    data() {
        return {
            links: [
                {
                    text: "Home",
                    url: "#",
                    current: false
                },
                {
                    text: "Courses",
                    url: "#",
                    current: false
                },
                {
                    text: "About Us",
                    url: "#",
                    current: false
                },
                {
                    text: "News",
                    url: "#",
                    current: false
                },
                {
                    text: "Pages",
                    url: "#",
                    current: false
                },
                {
                    text: "Contact",
                    url: "#",
                    current: false
                },
                {
                    text: "Purchase",
                    url: "#",
                    current: false
                }
            ]
        }
    },

    // methods: {
    //     changeCurrent() {
    //         this.links.forEach(el => {
    //             if (el.current === false)
    //                 el.current = true;
    //             else
    //                 el.current = false
    //         });
    //     }
    // }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/button.scss';
// My color
$yellow_clr: #E9D758;


// general
ul {
    display: inline-block;
}

.header_jumbo_container {
    background-image: url("../assets/img/theme_slider2_bg-1.jpg");
    height: 500px;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    font-weight: 700;
    color: white;

    .bg_color {
        background-color: rgba($color: #E56768, $alpha: 0.8);
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
    }

    .container_header {

        display: flex;
        justify-content: space-between;
        align-items: center;
        padding-top: 20px;

        img {
            width: 200px;
            margin: 0 20px;
        }

        ul {
            list-style-type: none;
            margin: 20px 0;

            li {
                display: inline-block;

                a {
                    color: white;
                    text-decoration: none;
                    padding: 0 10px;

                    &.active {
                        color: $yellow_clr;
                    }

                    &:hover {
                        color: $yellow_clr;
                    }
                }
            }
        }

    }

    .icon_down {
        font-size: 10px;
        margin-left: 5px;
        margin-bottom: 2px;
    }
}

.container_jumbo {
    width: 40%;
    margin: 0 auto;
    text-align: center;

    .title_jumbo {
        font-size: 50px;
        margin-top: 30px;
    }

    p {
        margin: 20px;
    }
}

.wave_container {
    position: relative;

    img {
        width: 100%;
        display: block;
        position: absolute;
        bottom: 0;
        left: 0;
    }
}
</style>
