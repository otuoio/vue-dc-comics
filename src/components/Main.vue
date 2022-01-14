<template>
  <main>
      <div class="main-content">
          <div class="container">
              <h1>&#8722;&#8722;&#62; Content goes here &#60;&#8722;&#8722;</h1>
          </div>
          
      </div>
      <div class="main-links">
          <div class="container">
              <div class="col">
                  <div class="icon">
                      <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                  </div>
                  <p>Digital comics</p>
              </div>
              <div class="col">
                  <div class="icon">
                      <img src="../assets/img/buy-comics-merchandise.png" alt="">
                  </div>
                  <p>Dc merchandise</p>
              </div>
              <div class="col">
                  <div class="icon">
                      <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                  </div>
                  <p>Comic shop locator</p>
              </div>
              <div class="col">
                  <div class="icon">
                      <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                  </div>
                  <p>Subscriptions</p>
              </div>
              <div class="col">
                  <div class="icon">
                      <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                  </div>
                  <p>Digital comics</p>
              </div>
          </div>
      </div>
  </main>
</template>

<script>
export default {
    name: "Main",
    data() {
        return {
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/partials/_variables.scss';

.main-content {
    background-color: $color-secondary;
    padding: 3em 0;
    .container h1 {
        font-size: 1em;
        font-weight: 700;
        color: white;
    }
}
.main-links {
    background-color: $color-primary;
    height: 150px;
    .container {
        display: flex;
        justify-content: space-around;
        align-items: center;
        .col {
            height: 100%;
            flex-basis: calc(100% / 6);
            margin-right: 2em;
            padding: 3em 0;
            display: flex;
            align-items: center;
            .icon {
                height: 60%;
                margin-right: 1em;
                img {
                    height: 100%;
                }
            }
            p {
                font-size: 0.8em;
                text-transform: uppercase;
                font-weight: 400;
                color: white;
            }
        }
    }
}

</style>