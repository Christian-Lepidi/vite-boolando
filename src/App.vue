<script>
import { store } from "./store/index";
import axios from "axios";

import AppHeader from "./AppHeader.vue";
import AppMain from "./AppMain.vue";
import AppFooter from "./AppFooter.vue";
import AppModal from "./components/AppModal.vue";

export default {
  data() {
    return {
      store,
      products: [],
    };
  },

  components: { AppHeader, AppMain, AppFooter, AppModal },

  created() {
    axios.get(`${store.apiUrl}/products`).then((resp) => {
      this.products = resp.data;
    });
  },
};
</script>

<template>
  <app-header></app-header>
  <app-modal v-if="store.modal.show"></app-modal>
  <app-main :products="products"></app-main>
  <app-footer></app-footer>
</template>

<style lang="scss">
@import "./styles/general.scss";
</style>
