<template>
  <div class="partners">
      <h2>OUR PARTNERS</h2>
      <div class="partner-logos">
        <div class="logo">
          <img alt="partner-logo" src="../assets/partner-logo-1.png">
        </div>

        <div class="logo">
          <img alt="partner-logo" src="../assets/partner-logo-2.png">
        </div>

        <div class="logo">
          <img alt="partner-logo" src="../assets/partner-logo-3.png">
        </div>

        <div class="logo">
          <img alt="partner-logo" src="../assets/partner-logo-4.png">
        </div>
      </div>
  </div>
</template>

<style lang="scss" scoped>
@import "../assets/sass/app.scss";

  .partners{
    display: flex;
    flex-flow: column;
    align-items: center;
    padding:5rem 2rem;
  }
  .partner-logos{
    width:80%;
    padding-top: 2rem;
    display: flex;
    justify-content: space-around;

      .logo{

        @include breakpoint(phablet){
          display: none;

          &:first-child{
            display: block;
          }
        }
      }
  }
</style>
