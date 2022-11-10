<template>
    <div class="sfondo">
        <div class="container">

            <div class="listone">
                <div>
                    <div class="primalista">
                        <h4>dc comics</h4>
                        <ul>

                            <li><a href="#nogo">Characters</a></li>
                            <li><a href="#nogo">Comics</a></li>
                            <li><a href="#nogo">Movies</a></li>
                            <li><a href="#nogo">TV</a></li>
                            <li><a href="#nogo">Games</a></li>
                            <li><a href="#nogo">Videos</a></li>
                            <li><a href="#nogo">News</a></li>
                        </ul>

                    </div>
                    <div class="secondalista">
                        <h4>shop</h4>
                        <ul>
                            <li><a href="#nogo">Shop DC</a></li>
                            <li><a href="#nogo">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                </div>
                <div class="terzalista">
                    <h4>DC</h4>
                    <ul>
                        <li><a href="#nogo">Term Of Use</a></li>
                        <li><a href="#nogo">Privacy policy (New)</a></li>
                        <li><a href="#nogo">Ad Choices</a></li>
                        <li><a href="#nogo">Advertising</a></li>
                        <li><a href="#nogo">Jobs</a></li>
                        <li><a href="#nogo">Subscription</a></li>
                        <li><a href="#nogo">Talent Workshops</a></li>
                        <li><a href="#nogo">CPSC Certificates</a></li>
                        <li><a href="#nogo">Ratings</a></li>
                        <li><a href="#nogo">Shop Help</a></li>
                        <li><a href="#nogo">Contact Us</a></li>
                    </ul>
                </div>
                <div class="quartalista">
                    <h4>Site</h4>
                    <ul>
                        <li><a href="#nogo">DC</a></li>
                        <li><a href="#nogo">AD Magazine</a></li>
                        <li><a href="#nogo">DC Kids</a></li>
                        <li><a href="#nogo">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </div>
            </div>
            <img src="../../public/img/dc-logo-bg.png" alt="">
        </div>
    </div>
    <div class="socials">
        <div class="container-socials">
            <a href="#nogo">sing up now</a>
            <div class="social">
                <span>Follow us</span>
                <img src="../../public/img/footer-facebook.png" alt="fb">
                <img src="../../public/img/footer-twitter.png" alt="twitter">
                <img src="../../public/img/footer-youtube.png" alt="yt">
                <img src="../../public/img/footer-pinterest.png" alt="pinterst">
                <img src="../../public/img/footer-periscope.png" alt="periscope">



            </div>
        </div>


    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/mixins' as *;
@use '../assets/style/partials/variabels' as *;

.sfondo {
    background-image: url(../../public/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    overflow-y: hidden;


    .container {
        @include dflex;
        height: 370px;

        .listone {
            display: flex;
        }

        h4 {
            color: $whitetext;
            text-transform: uppercase;
            font-size: 1.5em;
            margin-bottom: 10px;
        }

        .primalista {
            margin-bottom: 18px;

        }

        ul {
            color: $whitetext;
            margin-right: 30px;

            li {
                list-style: none;

                a {
                    color: $textgray;
                    text-decoration: none;

                    &:hover {
                        color: white;
                    }


                }
            }
        }
    }


}

.container-socials {
    display: flex;
    max-width: 1170px;
    margin: 0 auto;
    padding: 1rem;
    justify-content: space-between;
}

.socials {
    background-color: $bgfooter;
    padding: 25px;

    a {

        border: 3px solid $bluetext;
        padding: 8px;
        color: white;
        text-decoration: none;
        text-transform: uppercase;

        &:hover {
            background-color: $bluetext;
        }
    }

    .social {
        @include dflex;


        span {
            margin-right: 10px;
            color: $bluetext ;
            font-size: 2em;
        }

        img {
            margin: 0 10px;

            &:hover {
                filter: brightness(0) invert(1)
            }

        }
    }
}
</style>