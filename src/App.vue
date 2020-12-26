<template>
  <div id="app">
    <nav-bar />
    <first-section />
    <trust-section />
    <about-us />  
    <futured-products />
    <fr-as-qe />
    <the-testimonials />
    <the-footer />
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import FirstSection from "./view/FirstSection.vue";
import TrustSection from "./view/TrustSection.vue";
import AboutUs from "./components/AboutUsTab.vue";
import FuturedProducts from "./components/ProductsCarousel";
import FrAsQe from "./components/FrequentlyAQ";
import TheTestimonials from "./view/TheTestimonials";
import TheFooter from "./view/TheFooter";



export default {
  components: { NavBar, FirstSection, TrustSection, AboutUs, FuturedProducts, FrAsQe, TheTestimonials, TheFooter },
  name: "App",
};
</script>

<style>
.app{
  width: 100%;
}
</style>
