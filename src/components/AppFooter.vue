<script>
    export default {
    name: 'AppFooter',
}
</script>

<template>

    <footer>
        <section class="footer-links">
            <div class="container">
                <!-- DC Comics Links -->
                <div class="column">
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
                    <h4>SHOP</h4>
                    <ul>
                    <li><a href="#">Shop DC</a></li>
                    <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div class="column">
                    <h4>DC</h4>
                    <ul>
                    <li><a href="#">Terms Of Use</a></li>
                    <li><a href="#">Privacy policy (New)</a></li>
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
                <div class="column">
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
        </section>
        <section class="footer-bottom">
            <div class="container">
                <button>SIGN-UP NOW!</button>
                <div class="social-links">
                    <h4>FOLLOW US</h4>
                    <ul>
                        <li><a href="#"><img src="/img/footer-facebook.png" alt="Facebook"></a></li>
                        <li><a href="#"><img src="/img/footer-twitter.png" alt="Twitter"></a></li>
                        <li><a href="#"><img src="/img/footer-youtube.png" alt="YouTube"></a></li>
                        <li><a href="#"><img src="/img/footer-pinterest.png" alt="Pinterest"></a></li>
                        <li><a href="#"><img src="/img/footer-periscope.png" alt="Periscope"></a></li>
                    </ul>
                </div>
            </div>
        </section>
    </footer>

</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/mixings' as *;

.footer-links{
    padding: 30px 0;
    background-image: url('/img/footer-bg.jpg'), url('/img/dc-logo-bg.png');
    background-size: cover,30%;
    background-repeat: no-repeat;

    .container{
        display: flex;
    }

    .column {
        margin-right: 20px;

        h4 {
        font-size: 14px;
        margin-bottom: 10px;
        color: white;
        }

        ul {
        list-style: none;
        padding: 0;

        li {
            margin-bottom: 5px;

            a {
            color: #999;
            text-decoration: none;
            font-size: 12px;

            &:hover {
                color: #fff;
            }
            }
        }
        }
    }
}

.footer-bottom {
    background-color: #1a1a1a;
    color: #fff;
    padding: 30px 0;

    .container {
      display: flex;
      justify-content: space-between;
      align-items: center;

      button {
        background-color: #1a1a1a;
        color: #fff;
        border: solid 2px #026bb5;
        padding: 10px 20px;
        cursor: pointer;
        font-size: 14px;

        &:hover {
          background-color: #026bb5;
        }
      }

      .social-links {
        display: flex;
        align-items: center;

        h4 {
          margin-right: 10px;
          font-size: 14px;
          color: #026bb5;
        }

        ul {
          display: flex;
          list-style: none;
          padding: 0;

          li {
            margin-right: 10px;

            a {
              display: block;
              width: 24px;
              height: 24px;

              img {
                width: 100%;
                height: 100%;
              }
            }
            }
        }
        }
    }
}
</style>