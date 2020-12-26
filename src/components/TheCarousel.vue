<template>
    <swiper class="swiper" :options="swiperOption">
      <swiper-slide
        ><div class="card">
          <ul class="card__rating">
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
          </ul>
          <h4 class="card__title">CBD 500 mg Orange Flavor Tincture</h4>
          <div class="card__image"><img src="../assets/bottle1.png" /></div>
          <div class="card__footer">
            <div class="card__footer-price"><p>$49.99 USD</p></div>
            <div class="card__footer-btn"><p>Shop</p></div>
          </div>
        </div></swiper-slide
      >
      <swiper-slide
        ><div class="card">
          <ul class="card__rating">
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
          </ul>
          <h4 class="card__title">Black ICE CBD Muscle Rub 200 mg</h4>
          <div class="card__image"><img src="../assets/bottle2.png" /></div>
          <div class="card__footer">
            <div class="card__footer-price"><p>$49.99 USD</p></div>
            <div class="card__footer-btn"><p>Shop</p></div>
          </div>
        </div></swiper-slide
      >
      <swiper-slide
        ><div class="card">
          <ul class="card__rating">
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
          </ul>
          <h4 class="card__title">CBD+Curcumin Coffee 750 mg</h4>
          <div class="card__image"><img src="../assets/bottle3.png" /></div>
          <div class="card__footer">
            <div class="card__footer-price"><p>$79.99 USD</p></div>
            <div class="card__footer-btn"><p>Shop</p></div>
          </div>
        </div></swiper-slide
      >
      <swiper-slide
        ><div class="card">
          <ul class="card__rating">
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
          </ul>
          <h4 class="card__title">CBD 500 mg Orange Flavor Tincture</h4>
          <div class="card__image"><img src="../assets/bottle1.png" /></div>
          <div class="card__footer">
            <div class="card__footer-price"><p>$49.99 USD</p></div>
            <div class="card__footer-btn"><p>Shop</p></div>
          </div>
        </div></swiper-slide
      >
      <swiper-slide
        ><div class="card">
          <ul class="card__rating">
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
          </ul>
          <h4 class="card__title">CBD 500 mg Orange Flavor Tincture</h4>
          <div class="card__image"><img src="../assets/bottle1.png" /></div>
          <div class="card__footer">
            <div class="card__footer-price"><p>$49.99 USD</p></div>
            <div class="card__footer-btn"><p>Shop</p></div>
          </div>
        </div></swiper-slide
      >
      <swiper-slide
        ><div class="card">
          <ul class="card__rating">
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
            <li class="card__rating-star"><i class="fas fa-star"></i></li>
          </ul>
          <h4 class="card__title">CBD 500 mg Orange Flavor Tincture</h4>
          <div class="card__image"><img src="../assets/bottle1.png" /></div>
          <div class="card__footer">
            <div class="card__footer-price"><p>$49.99 USD</p></div>
            <div class="card__footer-btn"><p>Shop</p></div>
          </div>
        </div></swiper-slide
      >      
    </swiper>
</template>

<script>

import "../styles/library/swiper.css";

export default {

  data() {
    return {
       swiperOption: {
        slidesPerView: 3,
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

<style lang='scss' scoped>
@import "../styles/TheCarousel/styles.scss";
</style>