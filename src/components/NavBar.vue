<template>
  <div>
     <nav class="nav" v-scroll="handleScroll">
      <div class="nav-list">
        <ul class="nav__list-list">
          <li class="nav__list-item"><p>Home</p></li>
          <li class="nav__list-item"><p>Products</p></li>
          <li class="nav__list-item"><p>FAQs</p></li>
          <li class="nav__list-item">
            <p>Contact Us</p>
          </li>
        </ul>
      </div>
      <div class="nav__logo">
        <p>CBD</p>
      </div>
      <div class="nav__registration">
        <ul class="nav__registration-list">
          <li class="nav__registration-item">
            <p>login</p>
          </li>
          <li class="nav__registration-item">
            <p>
              <svg
                width="21"
                height="21"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                xmlns:svgjs="http://svgjs.com/svgjs"
                viewBox="0.004 0 20.992 21"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="21"
                  height="21"
                  viewBox="1.025 2 19.992 20"
                >
                  <path
                    paint-order="stroke fill markers"
                    fill-rule="evenodd"
                    d="M20.844 20.98l-4.86-4.86a8.494 8.494 0 0 0 2.094-5.593C18.078 5.823 14.25 2 9.55 2c-4.704 0-8.526 3.828-8.526 8.528 0 4.701 3.826 8.528 8.526 8.528a8.49 8.49 0 0 0 5.591-2.093l4.86 4.86a.584.584 0 0 0 .842 0 .6.6 0 0 0 0-.842zM2.218 10.527c0-4.044 3.29-7.33 7.329-7.33 4.044 0 7.33 3.29 7.33 7.33s-3.286 7.335-7.33 7.335c-4.04 0-7.33-3.29-7.33-7.335z"
                  />
                </svg>
              </svg>
              Search
            </p>
          </li>
          <li class="nav__registration-item">
            <p>Cart (0)</p>
          </li>
        </ul>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  directives: {},
  methods: {
    handleScroll: function(evt, el) {
      if (window.scrollY > 50) {
        el.setAttribute(
          "style",
          "background-color: #ffffff; opacity: 1; color: #413f3f; trnsition: all .5s ease; fill: none; "
        );
        return window.scrollY > 100;
      } else if (window.scrollY === 0) {
        el.setAttribute(
          "style",
          "background-color: transparent; opacity: .4; "
        );
        return window.scrollY === 0;
      }
      // return window.scrollY > 100;
    },
  },
  computed: {},
};
</script>

<style lang="scss" scoped>
svg {
  fill: #ffffff;
}
.nav {
  width: 100%;
  display: flex;
  position: fixed;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  top: 0;
  left: 0;
  border-bottom: 1px solid #ffffff;
  opacity: 0.4;
  z-index: 99;
  color: #ffffff;
  border-color: #ffffff;
  &__list-list {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
  }
  &__list-item {
    margin-right: 30px;
    font-family: "Oswald", sans-serif;
    font-weight: 400;
    font-size: 16px;
    text-transform: uppercase;
  }
  &__list-item:last-child {
    margin-right: 0;
  }
  &__logo {
    position: absolute;
    top: 16px;
    left: 50%;
    transform: translateX(-50%);
    font-family: "Oswald", sans-serif;
    font-weight: 400;
    font-size: 30px;
    text-transform: uppercase;
    // color: #ffffff;
    opacity: 0.6;
  }
  &__registration-list {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    height: 100%;
    padding-right: 30px;
  }
  &__registration-item {
    display: flex;
    align-items: center;
    padding-left: 30px;
    height: 78px;
    // border-left: 1px solid #ffffff;
    border-left: 1px solid;
    margin-right: 30px;
    font-family: "Oswald", sans-serif;
    font-weight: 400;
    font-size: 16px;
    text-transform: uppercase;
  }
  &__registration-item:last-child {
    margin-right: 0;
  }
  &__registration-item-icon {
    margin-right: 7px;
    transform: translateY(3px);
  }
}
</style>
