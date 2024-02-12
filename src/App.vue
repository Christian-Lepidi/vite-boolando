<script>
import axios from "axios";

import AppHeader from "./AppHeader.vue";
import AppMain from "./AppMain.vue";
import AppFooter from "./AppFooter.vue";

export default {
  data() {
    return {
      products: [],
    };
  },

  components: { AppHeader, AppMain, AppFooter },

  created() {
    axios.get("http://localhost:3000/products").then((resp) => {
      this.products = resp.data;
    });
  },
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
