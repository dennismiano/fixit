<template>
  <!--<img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>-->
  <Header/>
  <Hero/>

  <div class="value-proposition">
    <h2>One Call Can Solve All Your House Problems</h2>
    <img alt="telephone" src="./assets/telephone.svg">
    <h1>+254 (0) 722 123 456</h1>
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
  #app {
    font-family: 'Montserrat', sans-serif;
    margin:0;
  }
  h1,h2,h3,h4,h5,h6,p,a, ::placeholder{
    margin:0;
    font-family: 'Montserrat', sans-serif;
  }
  p, li{
    font-size: 0.8rem;
  }

  .value-proposition{
    display: flex;
    background-color: #faa21b;
    flex-flow: column;
    align-items: center;
    padding:2rem;
    height: 20rem;
    justify-content: center;
  }
  .value-proposition > img{
    width:5rem;
    height: 5rem;
  }
  .value-proposition > h1{
    font-weight: 800;
    font-size: 4rem;
  }
</style>
