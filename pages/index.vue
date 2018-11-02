<template>
  <div>
    <section>
      <div>
        <hero
          title="Rebekah and Clark"
          subtitle="February 16, 2019"
        />
      </div>
      <date />
      <img
        class="image container"
        src="~assets/hands.jpeg"
      >
      <location />
      <img
        class="image container"
        src="~assets/dark.jpeg"
      >
      <registry />
      <img
        class="image container"
        src="~assets/walk.jpeg"
      >
      <rsvp />
    </section>
  </div>
</template>

<script>
  import Hero from '~/components/Hero.vue';
  import Date from '~/components/Date.vue';
  import Location from '~/components/Location.vue';
  import Registry from '~/components/Registry.vue';
  import Rsvp from '~/components/Rsvp.vue';

  export default {
    components: {
      Hero,
      Date,
      Location,
      Registry,
      Rsvp
    }
  }
</script>

<style>
  h1.title {
    font-family: 'Reenie Beanie', cursive;
    font-size: 10vw;
    color: #707072;
  }

  h2.subtitle {
    font-family: 'Reenie Beanie', cursive;
    font-size: 7vw;
    color: #9c9c9c;
  }

  h3.subtitle {
    font-family: 'Reenie Beanie', cursive;
    font-size: 6vw;
    color: #9c9c9c;
  }

  .fullheight {
    height: 100vh;
  }
</style>
