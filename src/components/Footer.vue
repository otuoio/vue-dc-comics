<template>
  <footer>
      <div class="footer-top">
          <div class="container">
              <div class="dc-comics">
                  <h2>Dc comics</h2>
                  <ul>
                      <li><a href="#">Characters</a></li>
                      <li><a href="#">Comics</a></li>
                      <li><a href="#">Movies</a></li>
                      <li><a href="#">Tv</a></li>
                      <li><a href="#">Games</a></li>
                      <li><a href="#">Videos</a></li>
                      <li><a href="#">News</a></li>
                  </ul>
              </div>
              <div class="shop">
                  <h2>Shop</h2>
                  <ul>
                      <li><a href="#">Shop Dc</a></li>
                      <li><a href="#">Shop Dc Collectibles</a></li>
                  </ul>
              </div>
              <div class="dc">
                  <h2>Dc</h2>
                  <ul><li><a href="#">Term of use</a></li>
                      <li><a href="#">Policy</a></li>
                      <li><a href="#">Ad choice</a></li>
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
              <div class="sites">
                  <h2>Sites</h2>
                  <ul>
                      <li><a href="#">DC</a></li>
                      <li><a href="#">MAD Magazine</a></li>
                      <li><a href="#">DC Kids</a></li>
                      <li><a href="#">DC Universe</a></li>
                      <li><a href="#">DC Power Visa</a></li>
                  </ul>
              </div>
          </div>
      </div>
      <div class="footer-bottom">
          <div class="container">

          </div>
      </div>
  </footer>
</template>

<script>
export default {
    name: "Footer",
    data() {
        return {

        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/partials/_variables.scss';

.footer-top {
    background-image: url(../assets/img/footer-bg.jpg);
    height: 300px;
    overflow: hidden;
    .container {
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: right;
        background-size: contain;
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        align-content: flex-start;
        padding: 1em;
        .dc-comics {
            flex-basis: 70%;
            margin: .4em;
        }
        .shop {
            flex-basis: 20%;
            margin: .4em;
        }
        .dc {
            flex-basis: 90%;
            margin: .4em;
        }
        .sites {
            flex-basis: 90%;
            margin: .4em;
        }
        ul {
            list-style: none;
            li a {
                text-decoration: none;
                color: grey;
                font-size: 0.6em;
            }
        }
        h2 {
            font-size: 0.7em;
            font-weight: 700;
            color: white;
            text-transform: uppercase;
        }
    }
}
</style>