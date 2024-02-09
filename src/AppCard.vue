<script>
export default {
  props: {
    id: Number,
    frontImage: String,
    backImage: String,
    brand: String,
    name: String,
    price: Number,
    isInFavorites: Boolean,
  },
};
</script>

<template>
  <div class="card">
    <div>{{ brand }}</div>
    <div>{{ name }}</div>
    <div class="price">{{ price }}</div>

    <img :src="frontImage" alt="" />
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: 390px;
  height: 500px;
  background-color: aquamarine;
  margin: 10px;
  position: relative;
}

.price {
  color: red;
}
.cards .front-image {
  display: block;
}

.cards .back-image {
  display: none;
}

.cards:hover .front-image {
  display: none;
}

.cards:hover .back-image {
  display: block;
}
</style>
