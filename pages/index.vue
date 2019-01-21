<template lang="pug">
  div
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
      .colored__container
        h3 Hi, My name is Oluwatosin Edwards
        p Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed dox <br>tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis <br>nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        b-card#skills-card(title="Skills"
          tag="article"
          style="text-align:center;"
          class="mb-2")
          .card-left
            .card__icon
              i(class="fas fa-laptop" style="color:#6A2B7F")
            .card__description
              p Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed dox <br>tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis <br>nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
            .card__list
              ul
                li HTML
                li CSS
                li JavaScript
                li Vue JS
          //- .card-right
          //-   .card__icon
          //-     i(class="fas fa-igloo" style="color:#6A2B7F")
          //-   .card__description
          //-     p Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed dox <br>tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis <br>nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
          //-   .card__list
          //-     ul
          //-       li HTML
          //-       li CSS
    
    .middle-2
      h3 Projects
      p Here you can view some of my recent projects
    .bottom
    

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
@import url('https://use.fontawesome.com/releases/v5.6.3/css/all.css');
@import "assets/variables";

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
      padding-bottom: 3rem;
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
      outline: none;
    }
  }
}

.middle{
  .colored__container{
    background-image: linear-gradient(to bottom right,$purp, $pink);
    width: 100vw;
    height: 35rem;
    margin: 10rem 0 0 0;
    display: flex;
    flex-direction: column;
    color: #FFFFFF;
    align-items: center;
    h3 {
      padding: 2rem 0 2rem 0;
      font-family: Roboto-Bold;
      font-size: 2rem;
    }
    p {
      text-align: center;
    }
    #skills-card {
      display: flex;
      flex-direction: row;
      background-color: #fff;;
      color: $purp;
      width:80vw;
      height: fit-content;
      box-shadow: 0 0 6px 0 rgba(70,73,77,0.30);
      .card-left{
        // border-right-style: solid;
        display: flex;
        flex-direction: column;
        align-content: center;
        align-items: center;
        .card__list {
          ul {
            list-style-type: none;
            padding: 0;
          }
        }
      }
      .card-right {
        display: flex;
        flex-direction: column;
        align-content: center;
        align-items: center;
      }
    }
  }
}

.bottom {
   background-image: linear-gradient(to bottom right,$purp, $pink);
   height: 10rem;
}
</style>
