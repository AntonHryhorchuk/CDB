<template>
  <div class="container" id="faq">
    <h2 class="container__title">Frequently asked questions</h2>
    <the-collapse />
  </div>
</template>

<script>
import TheCollapse from "../components/TheCollapse.vue";
export default {
  components: { TheCollapse },
};
</script>
<style lang="scss" scoped>
@import "../styles/FAQ/styles.scss";
</style>
