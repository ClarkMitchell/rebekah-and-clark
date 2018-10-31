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
  export default {
    props: {
      title: {
        type: String,
        default: "Rebekah and Clark"
      },
      subtitle: {
        type: String,
        default: "February 16, 2019"
      }
    },
  }
</script>

<style scoped>
  h1.title {
    font-family: 'Dawning of a New Day', cursive;
    font-size: 10vw;
    color: rgba(255, 255, 255, 0.8);
  }

    h2.subtitle {
        font-family: 'Reenie Beanie', cursive;
        font-size: 7vw;
        color: rgba(255, 255, 255, 0.8);;
    }

  .has-bg-image {
    background: url("~assets/hero.jpeg") left center;
    background-size: cover;
  }
</style>