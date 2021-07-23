<template>
  <div class="booking-form">
      <div class="form-intro">
        <h2>Book a service</h2>
        <p>You can get started by entering a few details</p>
      </div>
      <input class="name" type="text" placeholder="full name">
      <input class="email" type="email" placeholder="email">
      <input class="number" type="number" placeholder="e.g +254 720 000 000">

      <select>
          <option value="0">-- Select type of service --</option>
          <option value="1">Plumbing</option>
          <option value="2">Electrical</option>
          <option value="3">Carpenty</option>
          <option value="4">Painting</option>
      </select>

      <input class="number" type="text" placeholder="Preffered date">

      <div class="book-button">
          <button type="button">Book Service</button>
      </div>
  </div>
</template>

<style lang="scss" scoped>

  @import "../assets/sass/app.scss";

  .booking-form{
    display: flex;
    flex-flow: column;
    width: 80%;
    background-color: $light-gray;
    padding:2rem;

    .form-intro{
      padding-bottom: 1rem;
    }
    input{
      @include form-inputs;
    }

      select{
      height: 2rem;
      margin-bottom:1rem;
      padding-left: 1rem;
      padding-right: 1rem;
      background-color: $light-gray;

      &::placeholder{
        color:#c3c3c3;
      }
    }

    button{
      @include button($primary-color, $white);
    }
    .name, .email, .number{
      //width:100%;
    }

  }

</style>
