<template>
    <header>
        <div class="header_jumbo_container">
            <div class="bg_color">
                <div class="container_header">
                    <a href="#"><img src="../assets/img/theme_eduprime_logo.png" alt="logo"></a>
                    <nav>
                        <ul>
                            <li v-for="(link, i) in links" :key="i">
                                <a :href="link.url" :class="link.current ? 'active' : ''">
                                    {{ link.text }}
                                </a>
                            </li>
                        </ul>

                        <button class="btn_yellow">
                            VIEW COURSES
                        </button>
                    </nav>

                </div>
            </div>

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
                    current: true
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
    }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
// My color
$yellow_clr: #E9D758;
.header_jumbo_container {
    background-image: url("../assets/img/theme_slider2_bg-1.jpg");
    height: 500px;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;

    .bg_color {
        background-color: #E56768;
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        opacity: 0.8;

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

        .btn_yellow{
            padding: 15px 25px;
            border-radius: 25px;
            color: white;
            background-color: $yellow_clr;
            border: none;
            margin: 0 20px;
        }

    }
}

ul{
    display: inline-block;
}

button {
    display: inline-block;
}
</style>
