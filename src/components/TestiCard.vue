<template>
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
</template>

<script>
import "../styles/library/swiper.css";
export default {
    data() {
    return {
      swiperOption: {
        slidesPerView: 1,
        spaceBetween: 30,
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
      },
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
    };
  },
}
</script>

<style lang='scss' scoped>
    @import "../styles/TestiCard/styles.scss";
</style>