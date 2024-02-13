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
emits:["open-card"],

};
</script>

<template>
  <div class="card" @click="$emit("open-card")">
    <img :src="'./img/' + frontImage" alt="" class="front-image" />
    <img :src="'./img/' + backImage" alt="" class="back-image" />
    <div>{{ brand }}</div>
    <div>{{ name }}</div>
    <div class="price">{{ price }}</div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: 390px;
  height: 500px;
  background-color: aquamarine;
  margin: 10px;
}

.price {
  color: red;
}
.card .front-image {
  display: block;
}

.card .back-image {
  display: none;
}

.card:hover .front-image {
  display: none;
}

.card:hover .back-image {
  display: block;
}
</style>
