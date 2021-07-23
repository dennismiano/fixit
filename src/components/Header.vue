<template>
  <Header/>

  <div class="header-wrapper">
    <div class="header-content">
      <img class="logo" alt="Vue logo" src="../assets/logo.svg">

      <div class="icons">
          <div class="icons-wrapper">
              <div class="icon">
                <img alt="clock" src="../assets/clock.svg">
              </div>
              <div class="icons-content">
                <h5>OPENING HOURS</h5>
                <p>Mon - Fri : 9 AM - 8 PM</p>
              </div>
          </div>

          <div class="icons-wrapper">
              <div class="icon">
                <img alt="call" src="../assets/call.svg">
              </div>

              <div class="icons-content">
                <h5>CALL US</h5>
                <p>+(10) 123 456 7966</p>
              </div>
          </div>

          <div class="icons-wrapper">
              <div class="icon">
                <img alt="mail" src="../assets/envelope.svg">
              </div>
              <div class="icons-content">
                <h5>MAIL US</h5>
                <p>Mon - Fri : 9 AM - 8 PM</p>
              </div>
          </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from './TopHeader.vue'

export default {
  name: 'HelloWorld',
  components:{
    Header
  },
  props: {
    msg: String
  }
}
</script>

<style lang="scss">
@import "../assets/sass/app.scss";
  .logo{
    height: 5rem;
    width: auto;
  }
  .header-wrapper{
    display: flex;
    justify-content: center;
    align-items: center;
    padding:1rem 0;
  }
  .header-content{
    width: 70%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .icons{
    display: flex;
    align-items: center;
  }
  .icons-wrapper{
    display: flex;
    margin-left: 1rem;

    &:first-child{
      margin-left: 0;
    }
  }
  .icon{
    width:3rem;
    background-color: #faa21b;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-right:.5rem;
  }
  .icon > img{
    width: 1rem;
  }
  .icons-content{
    p{
      color:$dark-gray;
    }
  }
</style>
