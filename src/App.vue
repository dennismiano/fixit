<template>
  <!--<img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>-->
  <Header/>
  <Hero/>

  <div class="value-proposition">
    <h2>One Call Can Solve All Your House Problems</h2>

    <div class="divider_wrapper">
      <img alt="telephone" src="./assets/stroke.svg">
      <img alt="telephone" src="./assets/telephone.svg">
      <img alt="telephone" src="./assets/stroke.svg">
    </div>

    <div class="number_wrapper">
      <h1>0722 - 123 - 456</h1>
    </div>

    <div class="appstore">
        <h3>You can also download our app</h3>
        <div class="app-icons">
            <img alt="telephone" src="./assets/applestore.svg">
            <img alt="telephone" src="./assets/playstore.svg">
        </div>
    </div>
  </div>

  <Partners/>
  <Footer/>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Footer from './components/Footer.vue'
import Partners from './components/Partners.vue'

export default {
  name: 'App',
  components: {
    //HelloWorld
    Header, Hero, Footer, Partners
  }
}
</script>

<style lang="scss">

@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800;900&display=swap');
@import "./assets/sass/app.scss";

  #app {
    font-family: 'Montserrat', sans-serif;
    margin:0;
  }

  //UTILITY CLASSES
  h1,h2,h3,h4,h5,h6,p,a, ::placeholder{
    margin:0;
    font-family: 'Montserrat', sans-serif;
  }
  p, li, a{
    font-size: 0.8rem;
  }



  .value-proposition{
    display: flex;
    background-color: #faa21b;
    flex-flow: column;
    align-items: center;
    padding:5rem 0rem;
    justify-content: center;

    @include breakpoint(phablet){
      margin-top: -3rem;
      padding-left: 1rem;
      padding-right:1rem;
    }
  }

  .value-proposition{
      h2{
        @include breakpoint(phablet){
          text-align: center;
          margin-top:2rem;
        }
      }
    .divider_wrapper{
      display: flex;
      align-items: center;
      justify-content: center;
      margin-top:2rem;

      @include breakpoint(phablet){
        margin-top:1rem;
      }

      img{
        height: 10px;

        @include breakpoint(phablet){
          height: 6px;
        }

        &:nth-child(2){
          width:5rem;
          height: 5rem;

          @include breakpoint(phablet){
            width:3rem;
            height: 3rem;
          }
        }
      }
    }
    .number_wrapper{
        h1{
          font-weight: 800;
          font-size: 5rem;

          @include breakpoint(phablet){
            font-size: 2rem;
            text-align: center;
          }
        }
    }

    .appstore{
        margin-top: 2rem;

        h3{
          text-align: center;
        }

      .app-icons{
        display: flex;
        margin-top:1rem;
        justify-content: center;

        img{
          height:3rem;
          width: auto;

          @include breakpoint(phablet){
            height:2.5rem;
          }

          &:last-child{
            margin-left:1rem;
          }
        }
      }
    }

  }
</style>
