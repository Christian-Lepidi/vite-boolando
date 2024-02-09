<script>
export default {
  props: {
    id: Number,
    frontImage: String,
    backImage: String,
    brand: String,
    name: String,
    isInFavorites: Boolean,
  },
};
</script>

<template></template>

<style lang="scss" scoped>
.cards {
  width: 390px;
  min-height: 500px;
  margin: 10px;
  position: relative;
}
</style>
