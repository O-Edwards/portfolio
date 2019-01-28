<template lang="pug">
  div
    .top
      .landing__image
        .title 
          h5#name I'm Oluwatosin Edwards
          h3#title I am a <br />Software Engineer
          a(href="#middle") <a>-</a> About Me
    .middle#middle
      .colored__container
        h3 Hi, My name is Oluwatosin Edwards
        p Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed dox <br>tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis <br>nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
    .middle-2
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
      h3 Projects
      p Here you can view some of my recent projects
      .project-list
        b-card(overlay
            img-src="https://www.idealtoy.co.za/assets/app/public/images/magento/coming_soon.jpg"
            img-alt="Card Image"
            text-variant="white"
            )
        b-card(overlay
            img-src="https://www.idealtoy.co.za/assets/app/public/images/magento/coming_soon.jpg"
            img-alt="Card Image"
            text-variant="white"
            )
        b-card(overlay
            img-src="https://www.idealtoy.co.za/assets/app/public/images/magento/coming_soon.jpg"
            img-alt="Card Image"
            text-variant="white"
            )
    .bottom
      b-card#contact-card(
        tag="article"
        style="text-align:center;"
        class="mb-2")
          h4 Contact methods
          p Hey hit me up
          b-button Contact
    

</template>

<script>

export default {
  components: {
  },
  computed: {
  },
  methods: {

  }
}
</script>

<style <style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Open+Sans:400,600');
@import url('https://use.fontawesome.com/releases/v5.6.3/css/all.css');
@import "assets/variables";

.top{ 
  display: flex;
  flex-direction: row;
  .landing__image {
    background: url(./assets/landing-image.svg) no-repeat;
    background-size: cover;
    width: 100vw;
    height: 100vh;
    display: flex;
    flex-direction: row;
    align-items: center;
    .title{
      margin-left: 12rem;
      h5 {
        font-family: 'Open Sans', sans-serif;
        color: white;
        font-size: 2rem;
        padding-bottom: 2rem;
      }
      h3 {
        font-family: 'Open Sans', sans-serif;
        display: block;
        font-weight: 600;
        font-size: 4rem;
        color: #fff;
        letter-spacing: 1px; 
        padding-bottom: 2rem;
      }
      a {
        color: #fff;
        a {
          &:hover{
            text-decoration: none;
          }
          color: #F68630;
          text-decoration: none;
        }
      }
    }
      
    }
  }


.middle{
  .colored__container{
    background-image: linear-gradient(to bottom right,$purp, $pink);
    width: 100vw;
    height: 20rem;
    margin: 0 0 0 0;
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
  }
}

.middle-2 {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 3rem;
  #skills-card {
      display: flex;
      flex-direction: row;
      background-color: #fff;;
      color: $purp;
      width:80vw;
      height: fit-content;
      box-shadow: 0 0 6px 0 rgba(70,73,77,0.30);
      margin: -6rem 0 4rem 0 !important;
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
  .project-list{
    & > *{
      width: 33.3%;
      margin: 0 2rem 2rem 2rem;
    }
    display: flex;
    flex-direction: row;
  }
}

.bottom {
  display: flex;
  justify-content: center;
  color: #fff;
  #contact-card {
    margin-top: -2rem;
    display: flex;
    justify-content: center;
    width: 60vw;
    max-height: 4.5rem;
    background-color: #293347;
    .card-body{
      display: flex;
      flex-direction: row;
      justify-content: space-evenly;
    }
  }
   background-image: linear-gradient(to bottom right,$purp, $pink);
   height: 15rem;
}
</style>
