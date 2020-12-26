<template>
  <div class="container">
    <swiper class="swiper" :options="swiperOption">
      <swiper-slide v-for="item in items" :key="item.text">
        <div class="card">
          <ul class="card__rating">
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
          </ul>
          <p class="card__text">{{ item.text }}</p>
          <h3 class="card__autor">{{ item.autor }}</h3>
          <div class="card__wrapper-bg-text">CBD every day</div>
        </div>
      </swiper-slide>
 
    </swiper>
         <div class="btn-holder">
        <div class="swiper-button-prev" slot="button-prev">
          <svg
            width="41"
            height="21"
            xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink"
            xmlns:svgjs="http://svgjs.com/svgjs"
            viewBox="0 0.254 41 20.492"
            fill="#ffffff"
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
            fill="#ffffff"
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
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";
export default {
  name: "swiper-example-multiple-slides-per-biew",
  title: "Multiple slides per view",
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      items: [
        {
          text:
            "I have tried another product after using this one successfully, and I am Back for good! The flavour, the lightness of the oil and the health benefits I have gotten with this oil are amazing!",
          autor: "Mark J.",
        },
        {
          text:
            "The first half of life consists of the capacity to enjoy without the chance, the last half consists of the chance without the capacity",
          autor: "Mark Twain",
        },
        { text: "While we are postponing, life speeds by.", autor: "Seneca" },
        {
          text: "If you do not think about the future, you cannot have one.",
          autor: "Galsworthy",
        },
      ],

      swiperOption: {
        slidesPerView: 1,
        spaceBetween: 30,
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
      },
    };
  },
};
</script>

<style lang="scss" scoped>
.container{
  position: relative;
  margin-bottom: 40px;
}
.card {
  position: relative;
  width: 100vw;
  min-height: 800px;
  // background-image: url("../assets/testi.png");
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url("../assets/testi.png");
  background-position: center;
  background-position-x: left;
  background-position-y: 76%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  text-align: center;
  // filter: brightness(60%);
  &__rating {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: row;
    padding-left: 0 !important;
    margin-bottom: 30px !important;
    &-star:not(:last-child) {
      margin-right: 5px;
    }
  }
  &__text {
    max-width: 700px;
    color: #ffffff;
    font-family: "Oswald", sans-serif;
    font-weight: 300;
    font-size: 16px;
    letter-spacing: 4px;
  }
  &__autor {
    position: relative;
    color: #ffffff;
    font-family: "Oswald", sans-serif;
    font-weight: 400;
    font-size: 20px;
    text-transform: uppercase;
    letter-spacing: 3px;
    &::before {
      position: absolute;
      content: " ";
      display: block;
      width: 40px;
      border-top: 2px solid #ffffff;
      top: 50%;
      left: -100%;
    }
  }
  &__wrapper-bg-text {
    position: absolute;
    left: -20px;
    bottom: 100px;
    font-family: "Oswald", sans-serif;
    font-weight: 300;
    font-size: 18px;
    text-transform: uppercase;
    color: #f7f8f3;
    opacity: 0.8;
    transform: rotate(90deg);
  }
}
.fa-star {
  color: #aab384;
}
img {
  fill: #ffffff;
}
.btn-holder {
  position: absolute;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: row;
  left: 50%;
  transform: translateX(-50%);
  bottom: 0;
  z-index: 99;
}
.swiper-button-prev{
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100px !important;
  height: 80px !important;
  border: 1px solid #ffffff;
}
.swiper-button-next{
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100px !important;
  height: 80px !important;
  border: 1px solid #ffffff;
} 
.swiper-button-next:focus{
     border:1px solid #ffffff;
    outline: none ;
  }
  .swiper-button-prev:focus{
     border: 1px solid #ffffff;
    outline: none ;
  }
</style>
