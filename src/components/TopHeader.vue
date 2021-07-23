<template>
    <div class="topheader">
      <div class="content">
        <a>Register</a>
        <a>Login</a>
      </div>
    </div>
</template>

<style lang="scss" scoped>
    @import "../assets/sass/app.scss";

    .topheader{
      background-color: $black-gray;
      display: flex;
      justify-content:center;
      padding: 0.3rem;

      .content{
        width:80%;
        display: flex;
        justify-content: flex-end;

        a{
          color:$white;

          &:last-child{
            margin-left:1rem;
          }
        }
      }
    }
</style>
