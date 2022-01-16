<template>
  <div class="card">
      <div class="thumb">
      <img :src="image" :alt="alt">
      </div>
      <h5>{{ text }}</h5>
  </div>
</template>

<script>
export default {
    name: "Card",
    props: {
        image: String,
        alt: String,
        text: String
    }
}
</script>

<style lang="scss" scoped>
    .card {
        flex-basis: calc((100%/6) - 1em);
        margin: .5em;
        .thumb {
        height: 160px;
        overflow: hidden;
        margin-bottom: .5em;
            img {
                width:100%;
            }
        }
        h5 {
            color: white;
            text-transform: uppercase;
        }
    }
</style>