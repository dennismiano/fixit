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
  .hero-wrapper{
    background-image: url('../assets/hero-bg-gradient.jpg');
    background-position: bottom center;
    background-size: cover;
    height: 500px;
    display: flex;
    justify-content: center;
  }
  .hero-content{
    display: flex;
    width:80%;

    .hero-image{
      width:50%;
      display: flex;
      justify-content: flex-end;
      align-items: flex-end;

      img{
        height: 100%;
        width: auto;
      }
    }
    .booking-form-wrapper{
      width:50%;
      display: flex;
      align-items: center;
    }
  }
</style>
