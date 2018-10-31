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
      <img src="/hands.jpeg">
      <location />
      <img src="/dark.jpeg">
      <registry />
      <img src="/walk.jpeg">
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
    font-family: 'Kaushan Script', cursive;
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

  .centered {
    padding-top: 10vh;
  }
</style>