<template>
  <main>
      <div class="main-content">
          <section class="jumbotron">
              <div class="message">Current series</div>
          </section>
          <div class="container">
              <div class="cards">
                  <Card v-for="(card, index) in cards"
                  :key="index"
                  :image="card.thumb"
                  :alt="card.series"
                  :text="card.series" />
              </div>
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
import Card from './Card.vue'

export default {
    name: "Main",
    components: {
        Card
    },
    data() {
        return {
            cards: [
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/partials/_variables.scss';

.main-content {
    background-color: $color-secondary;
    .jumbotron {
        height: 400px;
        background-image: url('../assets/img/jumbotron.jpg');
        background-size: cover;
        background-position: top;
        background-repeat: no-repeat;
        position: relative;
        .message {
            display: inline-block;
            background-color: $color-primary;
            color: white;
            text-transform: uppercase;
            font-size: .8em;
            font-weight: 700;
            padding: 1em 2em;
            position: absolute;
            bottom: 0;
            left: calc(35% / 2);
            transform: translate(-10%, 50%);
        }
    }
    .cards {
        display: flex;
        flex-wrap: wrap;
        padding: 2em;
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