<template>
  <section class="hero is-fullheight has-bg-image">
    <div class="hero-body">
      <div class="container">
        <h1 class="title has-text-centered">
          {{ title }}
        </h1>
        <h2 class="subtitle has-text-centered">
          {{ subtitle }}
        </h2>
      </div>
    </div>
  </section>
</template>

<script>
  import Parallax from 'vue-parallaxy';

  export default {
    props: ['title', 'subtitle'],
    components: {
      Parallax
    }
  }
</script>

<style scoped>
    h1.title {
        font-family: 'Kaushan Script', cursive;
        font-size: 10vw;
        color: white;
    }

    h2.subtitle {
        font-family: 'Reenie Beanie', cursive;
        font-size: 7vw;
        color: white;
    }

    .has-bg-image {
        background: url("~/assets/hero.jpeg") left center;
        background-size: cover;
    }
</style>