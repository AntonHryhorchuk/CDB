<template>
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
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    accordion: function(event) {
      var matches = document.querySelectorAll(".accordion__item-head");
      for (var i = 0; i < matches.length; i++) {
        matches[i].classList.remove("active");
      }

      event.target.classList.toggle("active");
    },
  },
};
</script>

<style lang='scss' scoped>
@import "../styles/TheCollapse/styles.scss";
</style>