<template>
  <div>
    <navbar />
    <nuxt/>
  </div>
</template>

<script>
  import Navbar from '~/components/Navbar.vue';

  export default {
    components: {
      Navbar
    }
  }
</script>

<style>
body {
  background-color: #F8F8F8;
}
</style>
