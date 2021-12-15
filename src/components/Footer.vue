<template>
    <footer>
        <!-- footer top -->
            <div class="top">
                <div class="container">
                    <ul>
                        <li>
                            <img id="digital" src="../assets/img/buy-comics-digital-comics.png" alt="">
                            <a href="#">Digital comics</a>
                        </li>
                        <li>
                            <img src="../assets/img/buy-comics-merchandise.png" alt="">
                            <a href="#">Dc merchandise</a>
                        </li>
                        <li>
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                            <a href="#">Subscription</a>
                        </li>
                        <li>
                            <img id="locator" src="../assets/img/buy-comics-shop-locator.png" alt="">
                            <a href="#">Comic shop location</a>
                        </li>
                        <li>
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                            <a href="#">Dc power visa</a>
                        </li>
                    </ul>
                </div>
            </div>
            <!-- /footer top -->

            <!-- footer center -->
            <div class="middle">
                <div class="container">
                    <div class="links">
                        <div class="col">
                            <ul>
                                <li><h3>dc comics</h3></li>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Comics</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">TV</a></li>
                                <li><a href="#">Games</a></li>
                                <li><a href="#">Videos</a></li>
                                <li><a href="#">News</a></li> 
                            </ul>
                            <ul>
                                <li><h3>shop</h3></li>
                                <li><a href="#">Shop DC</a></li>
                                <li><a href="#">Shop DC Collectibles</a></li>
                            </ul>
                        </div>
                        <div class="col">
                            <ul>
                                <li><h3>dc</h3></li>
                                <li><a href="#">Terms Of Use</a></li>
                                <li><a href="#">Privacy policy (New)</a></li>
                                <li><a href="#">Ad Choices</a></li>
                                <li><a href="#">Advertising</a></li>
                                <li><a href="#">Jobs</a></li>
                                <li><a href="#">Subscriptions</a></li>
                                <li><a href="#">Talent</a></li>
                                <li><a href="#">characters</a></li>
                            </ul>
                        </div>
                        <div class="col">
                            <ul>
                                <li><h3>sites</h3></li>
                                <li><a href="#">DC</a></li>
                                <li><a href="#">MAD Magazine</a></li>
                                <li><a href="#">DC Kids</a></li>
                                <li><a href="#">DC Universe</a></li>
                                <li><a href="#">DC Power Visa</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            <!-- /footer center -->

            <!-- footer bottom -->
            <div class="bottom">
                <div class="contaier">
                    <div class="divider">
                        <div class="sign-up">
                            <button>Sign-up now!</button>
                        </div>
                        <div class="social">
                            <div class="follow">
                                <p>Follow us</p>
                            </div>
                            <div class="icons">
                                <ul>
                                    <li>
                                        <a href="#">
                                            <img src="../assets/img/footer-facebook.png" alt="facebook">
                                        </a>
                                    </li>
                                    <li>
                                        <a href="#">
                                            <img src="../assets/img/footer-twitter.png" alt="twitter">
                                        </a>
                                    </li>
                                    <li>
                                        <a href="#">
                                            <img src="../assets/img/footer-youtube.png" alt="youtube">
                                        </a>
                                    </li>
                                    <li>
                                        <a href="#">
                                            <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                                        </a>
                                    </li>
                                    <li>
                                        <a href="#">
                                            <img src="../assets/img/footer-periscope.png" alt="periscope">
                                        </a>
                                    </li>
                                </ul>
                            </div>
                        </div>

                    </div>
                </div>
            </div>
            <!-- /footer bottom -->
    </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang = "scss" scoped>
@import '../assets/style/partials/variables.scss';
    .top .container{
        width: 100%;
    }
    .top {
        background-color: #0282F9;
        display: flex;
        ul {
            height: 100px;
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: space-evenly;
            list-style: none;
            li {
                display: flex;
                align-items: center;
                /* margin: 0 20px; */
                img {
                    width: 35px;
                }
                a {
                    text-decoration: none;
                    text-transform: uppercase;
                    font-size: 12px;
                    color: white;
                    margin-left: 10px;
                }
            }
        }
    }

    #locator{
        width: 25px;
    }
    #digital{
        width: 30px;
    }

    .middle {
        height: 300px;
        background-image: url('../assets/img/footer-bg.jpg');
        
    }

    .middle .container {
        height: 100%;
        display: flex;
        align-items: center;
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: right;
        background-size: 40%;
    }

    .links {
        display: flex;
        .col {
            margin-right: 30px;
            ul {
                list-style: none;
                margin-bottom: 15px;
                li h3 {
                    color: white;
                    text-transform: uppercase;
                }
                li a {
                    font-size: 13px;
                    color: #959595;
                    text-decoration: none;
                }
            }
        }
    }

    .bottom {
        background-color: $gray;
    }
    
    .divider {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 80px;
    }

    .sign-up button {
        background-color: $gray;
        color: white;
        text-transform: uppercase;
        padding: 10px;
        border: 2px solid $blue;
    }

    .social {
        display: flex;
        align-items: center;

        .follow {
            margin-right: 20px;
            p {
                text-transform: uppercase;
                font-weight: bold;
                color: $blue;
            }
        }

        .icons ul {
            list-style: none;
            li {
                display: inline-block;
                margin: 0 10px;
                a img {
                    width: 30px;
                }
           } 
        }
    }
</style>