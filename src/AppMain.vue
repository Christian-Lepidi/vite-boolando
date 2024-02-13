<script>
import AppCard from "./AppCard.vue";

export default {
  data() {
    return {
      products: [],
    };
  },

  props: Array,

  components: { AppCard },
};
</script>

<template>
  <main>
    <div class="container">
      <app-card
        v-for="product in products"
        :name="product.name"
        class="strong"
        :brand="product.brand"
        :price="product.price"
        :frontImage="product.frontImage"
        :backImage="product.backImage"
      />
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
