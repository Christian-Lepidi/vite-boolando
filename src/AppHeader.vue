<script>
export default {};
</script>

<template>
  <header class="header">
    <div class="header-container">
      <span class="text-header">donna uomo bambini</span>
      <img src="../cartella slack/img/boolean-logo.png" alt="" class="logo" />
      <div class="icons-header">
        <i class="far fa-user"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-shopping-bag"></i>
      </div>
    </div>
  </header>
</template>

<style scoped>
.header {
  width: 100%;
  height: 90px;
  background-color: orangered;
  position: sticky;
  top: 0;
  z-index: 1;
}

.header-container {
  width: 80%;
  height: 90px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.text-header {
  font-size: 20px;
  color: white;
}

.logo {
  height: 40px;
}

.icons-header {
  color: white;
}
</style>
