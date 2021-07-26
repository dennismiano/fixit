<template>
    <div class="hero-wrapper">
      <div class="hero-content">
          <div class="hero-image">
              <img alt="Vue logo" src="../assets/repairman.png">
          </div>

          <div class="booking-form-wrapper">
            <BookingForm/>
          </div>
      </div>
    </div>
</template>

<script>
  import BookingForm from './BookingForm.vue'

  export default {
    components: {
      //HelloWorld
      BookingForm
    }
  }
</script>

<style lang="scss" scoped>
@import "../assets/sass/app.scss";

  .hero-wrapper{
    background-image: url('../assets/hero-bg.jpg');
    background-position: bottom center;
    background-size: cover;
    //height: 500px;
    display: flex;
    justify-content: center;
  }
  .hero-content{
    display: flex;
    width:80%;

    @include breakpoint(phablet){
      flex-flow: column;
      width:100%;
      padding-left: 1rem;
      padding-right: 1rem;
      margin-top: -2rem;
    }

    .hero-image{
      width:50%;
      display: flex;
      justify-content: flex-end;
      align-items: flex-end;

      @include breakpoint(phablet){
        width:100%;
        height: 150px;
        justify-content: flex-start;
        align-items: flex-start;
      }

      img{
        height: 100%;
        width: auto;

        @include breakpoint(phablet){
          height: 150%;
        }
      }
    }
    .booking-form-wrapper{
      width:50%;
      display: flex;
      align-items: center;

      @include breakpoint(phablet){
        width:100%;
      }
    }
  }
</style>
