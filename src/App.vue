<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  data() {
    return {};
  },

  components: { AppHeader, AppMain, AppFooter },
};
</script>

<template>
  <p>
    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Alias,
    dolorum!<span>Lorem ipsum dolor sit amet consectetur adipisicing.</span>
  </p>
  <app-header></app-header>
  <app-main></app-main>
  <app-footer></app-footer>
</template>

<style lang="scss">
p {
  color: orange;

  span {
    color: aquamarine;
  }
}
</style>
