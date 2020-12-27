<template>
  <div class="container" id="products">
    <h2 class="container__title">CBD Featured Products</h2>
    <the-carousel/>
   <div class="btn-holder">
      <div class="swiper-button-prev" slot="button-prev">
        <svg
          width="41"
          height="21"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          xmlns:svgjs="http://svgjs.com/svgjs"
          viewBox="0 0.254 41 20.492"
          fill="#6e774a"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="41"
            height="21"
            viewBox="2.01 2.014 39.99 19.988"
          >
            <path
              paint-order="stroke fill markers"
              fill-rule="evenodd"
              d="M2.274 11.37l9.089-9.04a.912.912 0 0 1 1.281-.099.9.9 0 0 1 0 1.373L5.11 11.108h35.981c.502 0 .91.405.91.904 0 .5-.408.904-.91.904H5.11l7.534 7.494a.9.9 0 0 1 .1 1.275.912.912 0 0 1-1.381 0l-9.089-9.04a.9.9 0 0 1 0-1.275z"
            />
          </svg>
        </svg>
      </div>
      <div class="swiper-button-next" slot="button-next">
        <svg
          width="41"
          height="22"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          xmlns:svgjs="http://svgjs.com/svgjs"
          viewBox="0 0.706 41 20.588"
          fill="#6e774a"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="41"
            height="22"
            viewBox="2 1.951 39.99 20.081"
          >
            <path
              paint-order="stroke fill markers"
              fill-rule="evenodd"
              d="M41.726 11.352l-9.089-9.083a.909.909 0 1 0-1.281 1.28l7.534 7.54H2.909a.908.908 0 1 0 0 1.815h35.98l-7.533 7.53a.908.908 0 1 0 1.281 1.28l9.089-9.082a.908.908 0 0 0 0-1.28z"
            />
          </svg>
        </svg>
      </div>
    </div>
  </div>
</template>

<script>
  import TheCarousel from "../components/TheCarousel.vue"
 export default {
   components:{TheCarousel},
 };
</script>

<style lang="scss" scoped>
@import "../styles/ProductsCarousel/styles.scss";
</style>
