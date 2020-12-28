<template>
  <div class="container" id="contacts">
    <div class="footer">
      <h1 class="footer__logo">CBD</h1>

      <div class="footer__wrapper">
        <div class="footer__wrapper-left">
          <p>Privacy Policy Terms of Use Return Policy</p>
        </div>
        <div class="footer__wrapper-social">
          <ul class="footer__wrapper-social-list">
            <li class="footer__wrapper-social-list-item">
              <a href="https://uk-ua.facebook.com/" target="_blank"><img src="../assets/Facebook.svg" alt="" /></a>
            </li>
            <li class="footer__wrapper-social-list-item">
              <a href="https://twitter.com/" target="_blank"><img src="../assets/Twitter.svg" alt="" /></a>
            </li>
            <li class="footer__wrapper-social-list-item">
              <a href="https://www.youtube.com/" target="_blank"><img src="../assets/YouTube.svg" alt="" /></a>
            </li>
          </ul>
        </div>
        <div class="footer__wrapper-right">
          <p>SHIPPING INFO RETURNS / EXCHANGES CONTACT</p>
        </div>
      </div>
      <h2 class="footer__subscribe">Subscribe to Newsletter</h2>
      <form action="info" @submit="info">
        <input type="email" v-model=" message" placeholder="Email"/>
        <div class="button" type="submit" @click="info"><img src="../assets/ArrowSubm.svg"></div>
      </form>
      <p class="footer__text">© 2018. CbD health.</p>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      message: "",
    }
  },
  methods: {
    info() {
      this.message!="Email" ? this.$message.info(this.message) : this.$message.info("please enter correct Email");       
    },    
  },
  
};
</script>

<style lang="scss" scoped>
@import "../styles/Footer/styles.scss";

</style>
