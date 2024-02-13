<script>
import { store } from "../store/index";

export default {
  data() {
    return { store };
  },

  methods: {
    closeModal() {
      store.modal.show = false;
    },
  },
};
</script>

<template>
  <div class="layover">
    <div class="modal">
      <button class="btn" @click="closeModal()">Close</button>
    </div>
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

.modal {
  width: 80%;
  height: 90px;
  background-color: white;
  position: relative;
}

.btn {
  padding: 10px;
  background-color: rgb(71, 199, 199);
  border-radius: 15px;
  position: absolute;
  bottom: 3px;
  right: 3px;
}
</style>
