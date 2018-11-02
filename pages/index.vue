<template>
  <div>
    <section>
      <div>
        <hero
          title="Rebekah and Clark"
          subtitle="February 16, 2019"
        />
      </div>
      <img
        class="image container"
        src="~assets/dark.jpeg"
        id="mobile-date"
      >
      <date />
      <img
        class="image container"
        src="~assets/hands.jpeg"
        id="mobile-location"
      >
      <location />
      <img
        class="image container"
        src="~assets/sand.jpeg"
        id="mobile-registry"
      >
      <registry />
      <img
        class="image container"
        src="~assets/walk.jpeg"
        id="mobile-rsvp"
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
    font-size: 8vw;
    color: #707072;
  }

  h2.subtitle {
    font-family: 'Reenie Beanie', cursive;
    font-size: 5vw;
    color: #9c9c9c;
  }

  h3.subtitle {
    font-family: 'Reenie Beanie', cursive;
    font-size: 4vw;
    color: #9c9c9c;
  }

  @media only screen and (max-width : 768px) {
    h1.title {
      font-size: 11vw;
    }

    h2.subtitle {
      font-size: 8vw;
    }

    h3.subtitle {
      font-size: 7vw;
    }
  }

  .image.container:target {
    color:#2bbbb3;
    padding-top:52px;
  }

  .fullheight {
    height: 100vh;
  }
</style>
