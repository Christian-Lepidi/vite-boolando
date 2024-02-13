<script>
export default {
  data() {
    return {};
  },
};
</script>

<template>
  <div class="layover">
    <h1>Sono una modale</h1>
  </div>
</template>

<style lang="scss" scoped>
.layover {
  position: fixed;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;

  background-color: rgba(0, 0, 0, 0.8);

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 15px;
}
</style>
