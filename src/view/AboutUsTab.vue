<template>
  <section class="about-us">
    <div class="about-us__tabs">
      <the-tabs />
    </div>
  </section>
</template>

<script>
import TheTabs from "../components/TheTabs.vue";
export default {
  components: { TheTabs },
};
</script>

<style lang="scss" scoped>
@import "../styles/AboutUsTab/styles.scss";
</style>
