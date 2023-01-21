<script>
export default {
    name: "AppFooter"
}
</script>

<template>
    <footer>
        <section id="footer-top">
            <div class="container">
                <div class="row">
                    <div class="col">
                        <div>
                            <h4>DC COMICS</h4>
                            <ul>
                                <li><a href="#">Characters</a></li>
                                <li><a href="#">Comics</a></li>
                                <li><a href="#">Movies</a></li>
                                <li><a href="#">TV</a></li>
                                <li><a href="#">Games</a></li>
                                <li><a href="#">Videos</a></li>
                                <li><a href="#">News</a></li>
                            </ul>
                            <div>
                                <h4>SHOP</h4>
                                <ul>
                                    <li><a href="#">Shop DC</a></li>
                                    <li><a href="#">Shop DC Collectibles</a></li>
                                </ul>
                            </div>
                        </div>
                        <div>
                            <h4>DC</h4>
                            <ul>
                                <li><a href="#">Terms Of Use</a></li>
                                <li><a href="#">Privacy Policy (New)</a></li>
                                <li><a href="#">Ad Choices</a></li>
                                <li><a href="#">Advertising</a></li>
                                <li><a href="#">Jobs</a></li>
                                <li><a href="#">Subscriptions</a></li>
                                <li><a href="#">Talent Workshops</a></li>
                                <li><a href="#">CPSC Certificates</a></li>
                                <li><a href="#">Ratings</a></li>
                                <li><a href="#">Shop Help</a></li>
                                <li><a href="#">Contact Us</a></li>
                            </ul>
                        </div>
                        <div>
                            <h4>SITES</h4>
                            <ul>
                                <li><a href="#">DC</a></li>
                                <li><a href="#">MAD Magazine</a></li>
                                <li><a href="#">DC Kids</a></li>
                                <li><a href="#">DC Universe</a></li>
                                <li><a href="#">DC Power Visa</a></li>
                            </ul>
                        </div>
                    </div>
                    <div class="col">
                        <figure>
                            <img src="../assets/img/dc-logo-bg.png" alt="dc_logo_bg">
                        </figure>
                    </div>
                </div>
            </div>
        </section>
        <section id="footer-bottom">
            <div class="container">
                <nav class="footer-nav">
                    <a href="#">SIGN-UP NOW!</a>
                    <ul>
                        <li>
                            <a href="#">FOLLOW US</a>
                        </li>
                        <li><a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a></li>
                        <li><a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a></li>
                    </ul>
                </nav>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/mixins' as *;
@use '../assets/scss/partials/variables' as *;

#footer-top {
    min-height: 500px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    padding: 30px 0;

    .row {
        @include flex-between;

        .col:first-child {
            display: flex;
        }

        h4 {
            color: white;
            padding: 11px 0;
        }

        ul {
            margin-right: 20px;

            a {
                color: gray;
                font-size: 0.8rem;

                &:hover {
                    color: lightgrey
                }
            }

        }

        figure {
            height: 500px;
            width: 500px;
        }

    }


}

#footer-bottom {
    height: 120px;
    background-color: $darkergray;

    .footer-nav {
        @include flex-between;
        height: 100%;

        >a {
            color: white;
            padding: 20px;
            border: 2px solid $darkblue;
        }

        ul {
            display: flex;
            align-items: center;

            a {
                padding: 20px 10px;
                display: block;
                color: $darkblue;
            }
        }
    }
}
</style>