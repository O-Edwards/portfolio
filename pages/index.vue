<template lang="pug">
  div
    //- b-navbar(toggleable="md" type="dark" variant="info" sticky=true id="nav")
    //-   b-navbar-toggle(target="nav_collapse")
    //-   b-navbar-brand(href="#") Oluwatosin Edwards
    //-   b-collapse(is-nav id="nav_collapse")
    //-     b-navbar-nav
    //-       b-nav-item(href="#") Home
    //-       b-nav-item(href="#") Menu
    .top
      .landing__image
      .header__text
        .space__man
          img#man(src="./assets/moon-man.png")
        h1.title Welcome
        img#circles(src="./assets/circles.svg")
        h2.subtitle My name is Oluwatosin Edwards, and I am a Software Engineer.<br>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed dox <br>tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis <br>nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        button#contact Contact Me
    .middle
    
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
@import url('https://fonts.googleapis.com/css?family=Roboto:400,900');

.top{ 
  display: flex;
  flex-direction: row;
  .landing__image {
    position: absolute;
    right: 0;
    top: 0;
    background: url(./assets/landing-image.svg) no-repeat;
    width: 70vw;
    height: 50vw;
  }
  .header__text{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding-top: 10vh;
    padding-left: 5rem;
    .space__man{ 
      background: url(./assets/moon.png) no-repeat;
      width: 15vw;
      height: 30vh;
      display: flex;
      align-items: center;
       #man {
          width: 10vw;
          top: -10vh;
          position: relative;
          -webkit-animation: mover 1s infinite  alternate;
          animation: mover 1s infinite  alternate;
        }
        @-webkit-keyframes mover {
          0% { transform: translateY(0); }
          100% { transform: translateY(-10px); }
        }
        @keyframes mover {
          0% { transform: translateY(0); }
          100% { transform: translateY(-10px); }
        }
    }
    .title {
      font-family: 'Roboto', sans-serif;
      display: block;
      font-weight: 600;
      font-size: 5rem;
      color: #4AA2FF;
      letter-spacing: 1px;
      margin: 0;
    }
    #circles{
      width: 8vw;
      padding: 2rem 0rem 2rem 0rem;
    }
    .subtitle {
      font-weight: 300;
      font-size: 30px;
      color: #526488;
      padding-bottom: 15px;
    }
    #contact {
      background: url(./assets/button.svg) no-repeat;
      width: 12rem;
      height: 4rem;
      border: none;
      font-family: Roboto-Bold;
      font-size: 22px;
      color: #FFFFFF;
      text-align: center;
    }
  }
}
</style>
