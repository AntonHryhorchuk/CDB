<template>
  <div class="container">
    <div class="footer">
      <h1 class="footer__logo">CBD</h1>

      <div class="footer__wrapper">
        <div class="footer__wrapper-left">
          <p>Privacy Policy Terms of Use Return Policy</p>
        </div>
        <div class="footer__wrapper-social">
          <ul class="footer__wrapper-social-list">
            <li class="footer__wrapper-social-list-item">
              <img src="../assets/Facebook.svg" alt="" />
            </li>
            <li class="footer__wrapper-social-list-item">
              <img src="../assets/Twitter.svg" alt="" />
            </li>
            <li class="footer__wrapper-social-list-item">
              <img src="../assets/YouTube.svg" alt="" />
            </li>
          </ul>
        </div>
        <div class="footer__wrapper-right">
          <p>SHIPPING INFO RETURNS / EXCHANGES CONTACT</p>
        </div>
      </div>
      <h2 class="footer__subscribe">Subscribe to Newsletter</h2>
      <form action="" method="post">
        <input type="email" />
        <div class="button" type="submit"><img src="../assets/ArrowSubm.svg"></div>
      </form>
      <p class="footer__text">© 2018. CbD health.</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  width: 100%;
  padding: 50px 0px;
}
.footer {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  width: 100%;
  max-width: 1170px;
  &__logo {
    position: relative;
    font-family: "Oswald", sans-serif;
    font-weight: 400;
    font-size: 30px;
    text-transform: uppercase;
    color: #6e774a;
    &::before {
      position: absolute;
      content: " ";
      display: block;
      width: 370px;
      border-top: 2px solid #6e774a;
      top: 50%;
      left: -1000%;
    }
    &::after {
      position: absolute;
      content: " ";
      display: block;
      width: 370px;
      border-top: 2px solid #6e774a;
      top: 50%;
      left: 330%;
    }
  }
  &__wrapper {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 90%;
    flex-direction: row;
    &-left {
      width: 100%;
      max-width: 390px;
      padding: 50px 120px 20px 120px;
      font-family: "Oswald", sans-serif;
      font-weight: 300;
      font-size: 14px;
      text-transform: uppercase;
      color: #6e774a;
      letter-spacing: 3px;
      text-align: center;
    }
    &-social {
      height: 135px;
      flex-flow: column wrap;
      width: 100%;
      align-content: flex-start;
      &-list {
        position: relative;
        display: flex;
        align-items: flex-start;
        justify-content: space-around;
        flex-direction: row;
        padding-left: 0;
        &::before {
          position: absolute;
          content: " ";
          display: block;
          height: 55px;
          border-left: 2px solid #6e774a;
          top: 200%;
          left: 48%;
        }
      }
    }
    &-right {
      width: 100%;
      max-width: 390px;
      padding: 50px 120px 20px 120px;
      font-family: "Oswald", sans-serif;
      font-weight: 300;
      font-size: 14px;
      text-transform: uppercase;
      color: #6e774a;
      letter-spacing: 3px;
      text-align: center;
    }
  }
  &__subscribe {
    font-family: "Oswald", sans-serif;
    font-weight: 400;
    font-size: 18px;
    text-transform: uppercase;
    color: #1c1c1b;
    letter-spacing: 3px;
    margin-bottom: 30px;
  }
  &__text{
      font-family: "Oswald", sans-serif;
      font-weight: 300;
      font-size: 11px;
      text-transform: uppercase;
      color: #6e774a;
      letter-spacing: 2px;
  }
}
form {
  display: flex;
  flex-direction: row;
  margin-bottom: 60px;
}
input {
  outline: none;
  width: 200px;
  height: 40px;
  border-left: 1px solid #6e774a;
  border-top: 1px solid #6e774a;
  border-bottom: 1px solid #6e774a;
  background-color: transparent;
  padding: 0 15px;
}
.button {
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
  width: 70px;
  height: 40px;
  border-right: 1px solid #6e774a;
  border-top: 1px solid #6e774a;
  border-bottom: 1px solid #6e774a;
  background-color: transparent;
  &::before{
position: absolute;
          content: " ";
          display: block;
          height: 32px;
          border-left: 1px solid #6e774a;
          top: 3px;
          left: 0;      
  }
  &:hover{
      filter: brightness(50%);
  }
}
</style>
