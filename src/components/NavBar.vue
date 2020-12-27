<template>
  <div>
    <nav class="nav" v-bind:class="{ borderdarkpanel: windowTop }">
      <div class="nav-list">
        <ul class="nav__list-list">
          <li class="nav__list-item">
            <a v-bind:class="{ active: windowTop }" v-scroll-to="{ el: '#home' }">Home</a>
          </li>
          <li class="nav__list-item">
            <a v-bind:class="{ active: windowTop }" v-scroll-to="{ el: '#products' }">Products</a>
          </li>
          <li class="nav__list-item">
            <a v-bind:class="{ active: windowTop }" v-scroll-to="{ el: '#faq' }">FAQs</a>
          </li>
          <li class="nav__list-item">
            <a v-bind:class="{ active: windowTop }" v-scroll-to="{ el: '#contacts' }">Contact Us</a>
          </li>
        </ul>
      </div>
      <div class="nav__logo">
        <a v-scroll-to="{ el: '#home' }" v-bind:class="{ active: windowTop }">CBD</a>
      </div>
      <div class="nav__registration">
        <ul class="nav__registration-list">
          <li
            class="nav__registration-item"
            v-bind:class="{ borderdark: windowTop }"
          >

           
            <login-modal  />
          </li>
          <li
            class="nav__registration-item"
            v-bind:class="{ borderdark: windowTop }"
          >
            <a v-bind:class="{ active: windowTop }">
              <svg
               class="nav__list-item"
                v-bind:class="{ active: windowTop }"
                width="21"
                height="21"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                xmlns:svgjs="http://svgjs.com/svgjs"
                viewBox="0.004 0 20.992 21"
              >
                <svg
                  v-bind:class="{ active: windowTop }"
                  xmlns="http://www.w3.org/2000/svg"
                  width="21"
                  height="21"
                  viewBox="1.025 2 19.992 20"
                >
                  <path
                    v-bind:class="{ active: windowTop }"
                    paint-order="stroke fill markers"
                    fill-rule="evenodd"
                    d="M20.844 20.98l-4.86-4.86a8.494 8.494 0 0 0 2.094-5.593C18.078 5.823 14.25 2 9.55 2c-4.704 0-8.526 3.828-8.526 8.528 0 4.701 3.826 8.528 8.526 8.528a8.49 8.49 0 0 0 5.591-2.093l4.86 4.86a.584.584 0 0 0 .842 0 .6.6 0 0 0 0-.842zM2.218 10.527c0-4.044 3.29-7.33 7.329-7.33 4.044 0 7.33 3.29 7.33 7.33s-3.286 7.335-7.33 7.335c-4.04 0-7.33-3.29-7.33-7.335z"
                  />
                </svg>
              </svg>
              Search
            </a>
            
          </li>
          <li
            class="nav__registration-item"
            v-bind:class="{ borderdark: windowTop }"
          >
            <a v-bind:class="{ active: windowTop }">Cart (0)</a>
          </li>
        </ul>
      </div>
      <the-burger v-show="itemSize"></the-burger>
    </nav>
    

    <the-sidebar>
      <ul class="sidebar-panel-nav">
       <li><a href="#home" v-scroll-to="{ el: '#home' }">Home</a></li>
       <li><a href="#products" v-scroll-to="{ el: '#products' }">Products</a></li>
       <li><a href="#faqs" v-scroll-to="{ el: '#faq' }">FAQs</a></li>
       <li><a href="#contact" v-scroll-to="{ el: '#contacts' }">Contuct Us</a></li>
       <li><a href="#login">Login</a></li>
       <li><a href="#search">Search</a></li>
       <li><a href="#card">Card</a></li>

     </ul>
    </the-sidebar>  </div>
</template>

<script>
import LoginModal from './LoginModal.vue';
import TheBurger from './Menu/TheBurger.vue';


import TheSidebar from './Menu/TheSidebar.vue';
export default {
 
  data() {
    return {
    itemSize: false,
    
    windowTop: 0,
    };
  },
  components:{LoginModal, TheBurger, TheSidebar,},
  mounted() {
    window.addEventListener("scroll", this.onScroll);
  },
  beforeDestroy() {
    window.removeEventListener("scroll", this.onScroll);
    window.removeEventListener('resize', this.onResize);
  },
  created() {
  window.addEventListener('resize', this.onResize);
  this.onResize();
},
  methods: {
    onResize() {
    this.itemSize = document.documentElement.clientWidth > 680 ? false : true;
  },
    onScroll(e) {
      this.windowTop = e.target.documentElement.scrollTop;
     
    },
  },
  computed: {
    Scroll: function() {
      return window.scrollY > 50 ? true : false;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../styles/NavBar/styles.scss";

</style>
