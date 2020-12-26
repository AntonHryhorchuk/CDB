<template>
  <div class="container">
    <h2 class="container__title">Frequently asked questions</h2>
    <div class="accordion" id="accordion">
      <div class="accordion__item">
        <img class="accordion__item-icon" src="../assets/plus.svg" />
        <h3 class="accordion__item-head" v-on:click="accordion">
          What is Cannabidiol (CBD)?
        </h3>

        <div class="accordion__item-body">
          <p class="accordion__item-text">
            Because CBD from hemp has no psychoactive effects, the purchase,
            sales, or possession of hemp CBD products are completely legal in
            all 50 States.
          </p>
        </div>
      </div>

      <div class="accordion__item">
        <img class="accordion__item-icon" src="../assets/plus.svg"/>
        <h3 class="accordion__item-head" v-on:click="accordion">
          Is Hemp-Derived Cannabidiol (CBD) Legal?
        </h3>
        <div class="accordion__item-body">
          <p class="accordion__item-text">
            Because CBD from hemp has no psychoactive effects, the purchase
          </p>
        </div>
      </div>

      <div class="accordion__item">
        <img class="accordion__item-icon" src="../assets/plus.svg" />
        <h3 class="accordion__item-head" v-on:click="accordion">
          Are there any negative side effects?
        </h3>
        <div class="accordion__item-body">
          <p class="accordion__item-text">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Blanditiis
            fuga excepturi molestias minus et odio deserunt quibusdam cumque
            odit aliquam tenetur possimus similique perferendis, quae incidunt
            praesentium porro exercitationem neque.
          </p>
        </div>
      </div>

      <div class="accordion__item">
        <img class="accordion__item-icon" src="../assets/plus.svg" />
        <h3 class="accordion__item-head" v-on:click="accordion">
          Do you offer a return policy?
        </h3>
        <div class="accordion__item-body">
          <p class="accordion__item-text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum
            reiciendis libero et voluptatem quia accusamus accusantium tempora
            velit vitae amet. Velit minima laudantium vero assumenda aperiam
            tenetur debitis accusamus fugiat?
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    accordion: function(event) {
      //Раскомментировать, если нужно, чтобы закрывались остальные пункты при открытии текущего
      var matches = document.querySelectorAll(".accordion__item-head");
      for (var i = 0; i < matches.length; i++) {
        matches[i].classList.remove("active");
      }

      event.target.classList.toggle("active");
    },
  },
};
</script>
<style lang="scss" scoped>
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  width: 100%;
  margin-bottom: 100px;
  &__title {
    color: #1c1c1b;
    font-family: "Oswald", sans-serif;
    font-weight: 400;
    font-size: 30px;
    text-transform: uppercase;
    letter-spacing: 4px;
    margin-bottom: 60px;
  }
}
.accordion {
  width: 100%;
  max-width: 570px;
  border-bottom: 2px solid #eaedde;
  margin-bottom: 50px;
  &__item {
    position: relative;
    
    &-icon {
      position: absolute;
      top: 15px;
      left: 0;
      z-index: 99;      
    }
    &-head {
      position: relative;
      background-color: #f7f8f3;
      cursor: pointer;
      padding: 10px 40px;
      border-top: 2px solid #eaedde;
      font-family: "Oswald", sans-serif;
      font-weight: 300;
      font-size: 18px;
      color: #6e774a;
      letter-spacing: 5px;
      &:hover{
        color:  #98a079;
        transition: all .3s ease;
      }
    }
    &-text{
      font-family: "Oswald", sans-serif;
      font-weight: 300;
      font-size: 18px;
      color:#000000;
    }
    &-body {
      display: none;
      padding: 20px 40px;
    }
  }
}

.accordion__item-head.active + .accordion__item-body {
  display: block !important;
}
</style>
