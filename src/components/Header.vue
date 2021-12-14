<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="logo">
            </div>
            <nav>
                <ul>
                    <!-- <li><a href="#"></a></li> -->
                    <li v-for="(link, index) in links" :key="index"><a :class="{ active: link.current }" :href="link.url">{{link.text}}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            // dati del componente
            links: [
                {
                    text: "characters",
                    url: "#",
                    current: true,
                },
                {
                    text: "comics",
                    url: "#",
                    current: false,
                },
                {
                    text: "movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "tv",
                    url: "#",
                    current: false,
                },
                                {
                    text: "games",
                    url: "#",
                    current: false,
                },
                                {
                    text: "collectibles",
                    url: "#",
                    current: false,
                },
                                {
                    text: "videos",
                    url: "#",
                    current: false,
                },
                                {
                    text: "fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "news",
                    url: "#",
                    current: false,
                },
                {
                    text: "shop",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';
    header{
       height: 100px; 
       padding-top: 10px;
    }
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .logo {
        padding: 0px 20% 0px 0;
    }
    .logo img{
        height: 70px;
    }
    nav {
        ul {
            display: flex;
            list-style: none;
            li {
                .active, :hover {
                    border-bottom: 5px solid;
                    color: $blue;
                };
                padding: 0px 20px;
                a {
                    display: inline-block;
                    text-decoration: none;
                    color: #000;
                    text-transform: uppercase;
                    line-height: 85px;
                };
            };
            
        };
    }
</style>