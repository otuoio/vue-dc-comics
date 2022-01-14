<template>
  <div class="card">
      <img :src="image" :alt="alt">
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

<style >

</style>