<template>
  <header>
      <div class="header-top"></div>
      <div class="header-bottom">
            <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <nav class="nav-menu">
                <ul>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#" class="active">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">Tv</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Collectibles</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">Fans</a></li>
                    <li><a href="#">News</a></li>
                    <li><a href="#">Shop</a></li>
                </ul>
            </nav>
        </div>
      </div>
      
  </header>
</template>

<script>
export default {
    name: "Header",
    data() {
        return {

        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/partials/_variables.scss';
    .header-top {
        width: 100%;
        height: 20px;
        background-color: black;
    }

    .header-bottom {
        height: 100px;
        width: 100%;
        background-color: white;
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1em;
            .logo {
                height: 100%;
                flex-basis: 40%;
                display: flex;
                align-items: center;
                img {
                    display: block;
                    height: 70%;
                }
            }
            .nav-menu {
                flex-basis: 60%;
                ul {
                    list-style: none;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    li a {
                        text-decoration: none;
                        color: gray;
                        padding: 1em;
                        text-transform: uppercase;
                        font-size: 0.7em;
                        font-weight: 700;
                        &:hover,
                        &:active,
                        &.active {
                            color: $color-primary;
                            border-bottom: 2px solid $color-primary;
                        }
                    }
                }
            }
        }
    }
</style>