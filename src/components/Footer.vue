<template>
    <div class="footer">
        <div class="footer-content">
            <div class="column">
                <h2>ABOUT FIXIT</h2>
                <p>That this group would somehow form a family that's the way we all became the Brady Bunch. Doin' it our way. There's nothing we wont try never heard word.</p>
                <a>Read More...</a>
            </div>

            <div class="column">
                <h2>USEFUL LINKS</h2>
                <li>About us</li>
                <li>FAQ</li>
            </div>

            <div class="column">
                <h2>OPENING HOURS</h2>
                <p>Monday - 9:00AM to 6:00PM</p>
                <p>Tuesday - 9:00AM to 6:00PM</p>
                <p>Wednesay - 9:00AM to 6:00PM</p>
                <p>Thursday - 9:00AM to 6:00PM</p>
                <p>Friday - 9:00AM to 6:00PM</p>
                <p>Saturday - 9:00AM to 6:00PM</p>
            </div>

            <div class="column">
                <h2>CONTACTS</h2>
                <p>Address:
                    44 New Design Street,
                    <br/>Melbourne 005</p>
                <p>Phone: +48 122 33 44 555</p>
                <p>Email: info@example.com</p>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import "../assets/sass/app.scss";

  .footer{
    background-image: url('../assets/footer-bg.svg');
    background-size: cover;
    background-position: center;
    display: flex;
    justify-content: center;
    padding:10rem 2rem;

    @include breakpoint(phablet){
      padding:3rem 2rem;
    }

    h2{
      font-weight: 600;
    }
    h2,p,li{
      color:white;
      margin-bottom: 1rem;
    }
  }
  .footer-content{
    display: flex;
    width:80%;

    @include breakpoint(phablet){
      width:100%;
      flex-flow: column;
    }

    .column{
      width:23.5%;
      margin-right: 2%;

      @include breakpoint(phablet){
        width:100%;
        margin-right: 0;
        margin-top:1rem;
      }

      &:last-child{
        margin-right: 0;
      }
    }
  }
</style>
