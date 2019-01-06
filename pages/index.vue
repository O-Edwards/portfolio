<template lang="pug">
  div
    //- b-navbar(toggleable="md" type="dark" variant="info" sticky=true)
      b-navbar-toggle(target="nav_collapse")
      b-navbar-brand(href="#") Oluwatosin Edwards
      b-collapse(is-nav id="nav_collapse")
        b-navbar-nav
          b-nav-item(href="#") Home
          b-nav-item(href="#") Menu
    .alignment__container
      .header__text
        //- h1 Hi! Welcome to My Portfolio Site
      .container__hero
        img#space(src="./assets/portfolio-hero.svg")
    .container
      logo
      h1.title
        ac-petersen
      h2.subtitle
        | Site for My Portfolio
      div.links
        a.button--green(href="https://nuxtjs.org/" target="_blank") Documentation
        a.button--grey(href="https://github.com/nuxt/nuxt.js" target="_blank") GitHub

</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
#space{
  top: 0px;
  right: 0px;
  position: absolute;
}
.alignment__container {
  display: flex;
  flex-direction: row;
}
.container {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.container__hero {
  
}

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

.links {
  padding-top: 15px;
}
</style>
