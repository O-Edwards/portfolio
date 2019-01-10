<template lang="pug">
  div
    b-navbar(toggleable="md" type="dark" variant="info" sticky=true id="nav")
      b-navbar-toggle(target="nav_collapse")
      b-navbar-brand(href="#") Oluwatosin Edwards
      b-collapse(is-nav id="nav_collapse")
        b-navbar-nav
          b-nav-item(href="#") Home
          b-nav-item(href="#") Menu
    .top
      .illustration
      .header__text
        h1.title portfolio
        h2.subtitle Welcome to my portfolio
    .portfolio
    .contact
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  computed: {
  },
  methods: {

  }
}
</script>

<style <style lang="scss" scoped>
@media(max-width: 1200px){
  .illustration {
      width: 700px;
      background-size: 700px;
  }
}

.top{ 
  display: flex;
  flex-direction: row;
  .illustration {
    width: 820px;
    height: 667px;
    position: absolute;
    right: 0;
    top: 0;
    background: url(./assets/portfolio-hero.svg) no-repeat;
    z-index: 2;
  }
  .header__text{
    .title {
      font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
        'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
      display: block;
      font-weight: 300;
      font-size: 100px;
      color: #35495e;
      letter-spacing: 1px;
    }
    .subtitle {
      font-weight: 300;
      font-size: 42px;
      color: #526488;
      word-spacing: 5px;
      padding-bottom: 15px;
    }
  }
}
</style>
