<template>
  <div id="navbar">
    <section class="is-fullheight is-bold">
      <nav class="navbar is-fixed-top is-transparent">
          <div class="navbar-brand">
            <a class="navbar-item" href="/">
              <img src="~/assets/celtic-heart.png" alt="Logo">
            </a>
            <div class="navbar-burger" @click="showNav = !showNav" :class="{ 'is-active': showNav }">
              <span></span>
              <span></span>
              <span></span>
            </div>
          </div>
          <div class="navbar-menu" :class="{ 'is-active': showNav }">
            <div class="navbar-end">
              <a
                v-for="(link, index) in links"
                :key=index
                class="navbar-item has-text-centered"
                :href=link.url
              >
                {{ link.title }}
              </a>
            </div>
          </div>
        </nav>
    </section>
  </div>
</template>

<script>
  export default {
    data: function() {
      return {
        showNav: false,
        links: [
          {
            title: "Date",
            url: "#date"
          },
          {
            title: "Location",
            url: "#location"
          },
          {
            title: "Registry",
            url: "#registry"
          },
          {
            title: "RSVP",
            url: "#rsvp"
          }
        ]
      }
    }
  }

</script>

<style>
  .navbar-item {
    color:#4a4a4a !important;
  }

  .is-transparent {
    background-color: rgba(0, 0, 0, 0);
  }

  .navbar-menu.is-active {
    background-color: rgba(0, 0, 0, .1);
  }
</style>
