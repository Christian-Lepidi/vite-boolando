<script>
import AppCard from "./AppCard.vue";

export default {
  data() {
    return {};
  },

  props: { products: Array },

  components: { AppCard },
};
</script>

<template>
  <main>
    <div class="container">
      <app-card v-for="product in products" class="strong" v-bind="product" />
    </div>
  </main>
</template>

<style lang="scss" scoped>
img {
  max-width: 100%;
  display: block;
}
.container {
  max-width: 80%;
  min-height: 1300px;
  margin: 0 auto;
  padding: 0 15px;
  display: flex;
  flex-wrap: wrap;

  .strong {
    text-transform: uppercase;
  }
}
</style>
