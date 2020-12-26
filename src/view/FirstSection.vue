<template>
  <section class="first-section">
    <div class="first-section__shadow"></div>

    <div class="first-section__wrapper">
      <p class="first-section__wrapper-title">Enhancing Life</p>
      <p class="first-section__wrapper-title">Excelling in Care</p>
      <h2 class="first-section__wrapper-subtitle">
        Choose Wisely. Choose CBD.
      </h2>
      <button class="first-section__wrapper-btn">Start Shopping</button>
      <a class="first-section__wrapper-link" href="">
        See all Products
        <svg
          width="21"
          height="11"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          xmlns:svgjs="http://svgjs.com/svgjs"
          viewBox="0 0.244 21 10.512"
          fill="#f7f8f3"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="21"
            height="11"
            viewBox="2 1.976 19.995 10.009"
          >
            <path
              paint-order="stroke fill markers"
              fill-rule="evenodd"
              d="M21.863 6.661l-4.544-4.527a.455.455 0 0 0-.641-.05.451.451 0 0 0 0 .688l3.767 3.758H2.455a.453.453 0 1 0 0 .905h17.99l-3.767 3.753a.452.452 0 0 0-.05.639.455.455 0 0 0 .69 0L21.864 7.3a.452.452 0 0 0 0-.639z"
            />
          </svg>
        </svg>
      </a>
    </div>
    <div class="first-section__wrapper-bg-text">CBD Potion health</div>
    <div class="first-section__scroll-icon">
      <a>
        <svg
          width="31"
          height="17"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          xmlns:svgjs="http://svgjs.com/svgjs"
          viewBox="0 0.233 31 16.535"
          fill="#fff"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="31"
            height="17"
            viewBox="1.994 1.994 30.008 16.005"
          >
            <path
              paint-order="stroke fill markers"
              fill-rule="evenodd"
              d="M31.695 2.304a1.063 1.063 0 0 0-1.499 0l-13.183 13.17-13.21-13.17a1.063 1.063 0 0 0-1.498 0 1.055 1.055 0 0 0 0 1.494L16.237 17.69c.207.206.466.31.75.31.258 0 .543-.104.75-.31L31.669 3.798c.44-.412.44-1.082.026-1.494z"
            />
          </svg>
        </svg>
      </a>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.first-section {
  position: relative;
  width: 100%;
  max-width: 100vw;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background-image: url("../assets/ImgBg.png");
  background-position: center;
  background-repeat: no-repeat;
  &__shadow {
    position: absolute;
    width: 100%;
    height: 277px;
    background-image: url("../assets/ShadowBg.png");
    background-position: center;
    background-repeat: no-repeat;
    top: 0;
    left: 0;    
  }
  &__wrapper-bg-text {
    position: absolute;
    left: -30px;
    bottom: 200px;
    font-family: "Oswald", sans-serif;
    font-weight: 400;
    font-size: 22px;
    text-transform: uppercase;
    color: #ffffff;
    opacity: 0.8;
    transform: rotate(-90deg);
  }
  &__wrapper-bg-text::before {
    content: "";
    display: block;
    width: 140px;
    border-top: 2px solid #ffffff;
    position: absolute;
    left: -170px;
    bottom: 15px;
  }
  &__wrapper {
    width: 100%;
    max-width: 768px;
    display: flex;
    align-items: flex-end;
    justify-content: center;
    flex-direction: column;
  }
  &__wrapper-title {
    font-family: "Oswald", sans-serif;
    font-weight: 400;
    font-size: 45px;
    text-transform: uppercase;
    color: #ffffff;
    letter-spacing: 5.2px;
  }
  &__wrapper-subtitle {
    font-family: "Oswald", sans-serif;
    font-weight: 400;
    font-size: 18px;
    color: #ffffff;
    margin-top: 30px;
    letter-spacing: 3px;
    margin-bottom: 25px;
  }
  &__wrapper-btn {
    position: relative;
    width: 200px;
    height: 40px;
    border: 1px solid #ffffff;
    background-color: inherit;
    color: #ffffff;
    font-family: "Oswald", sans-serif;
    font-weight: 400;
    font-size: 18px;
    text-transform: uppercase;
    text-align: start;
    padding-left: 20px;
    margin-bottom: 20px;
  }
  &__wrapper-btn::before {
    position: absolute;
    content: "";
    width: 30px;
    border-top: 2px solid #ffffff;
    top: 50%;
    left: 75%;
  }
  &__wrapper-link-icon {
    margin-left: 20px;
  }
  &__wrapper-link {
    color: #ffffff;
    font-family: "Oswald", sans-serif;
    font-weight: 400;
    font-size: 14px;
    letter-spacing: 2px;
  }
  &__scroll-icon {
    position: absolute;
    left: 50%;
    bottom: 3%;
    transform: translateX(-50%);
  }
}
</style>
