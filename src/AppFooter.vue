<script>
export default {};
</script>

<template>
  <footer class="footer">
    <div class="footer-container">
      <div>
        <h4 class="h4">Boolando s.r.l.</h4>
        <a href="#" class="link">infomazioni legali</a>
        <a href="#" class="link">infomativa privacy</a>
        <a href="#" class="link">diritto di recesso</a>
      </div>
      <span class="info">Trovaci anche su</span>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
.footer {
  width: 100%;
  height: 120px;
  background-color: rgb(34, 34, 34);
}

.footer-container {
  width: 80%;
  height: 120px;
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.h4 {
  font-size: 18px;
  color: white;
  margin-bottom: 5px;
}
.link {
  text-decoration: none;
  color: white;
}

.info {
  font-size: 18px;
  color: white;
  margin-right: 0;
}
</style>
