<script>
import AppHeader from "./AppHeader.vue";
import AppMain from "./AppMain.vue";
import AppFooter from "./AppFooter.vue";

export default {
  data() {
    return {};
  },

  components: { AppHeader, AppMain, AppFooter },
};
</script>

<template>
  <app-header></app-header>
  <app-main></app-main>
  <app-footer></app-footer>
</template>

<style lang="scss">
@import "./styles/general.scss";
</style>
