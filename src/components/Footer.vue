<script setup>

</script>

<template>
  <footer class="footer">
    <div>
      <img class="footer__logo" src="../assets/twitter.png" alt="">
      <img class="footer__logo" src="../assets/facebook.png" alt="">
      <img class="footer__logo" src="../assets/instagram.png" alt="">
    </div>

  </footer>
</template>

<style scoped>
.footer {
  height: 100px;
  background: #f4a261;
  display: flex;
  justify-content: center;
  align-items: center;
}
.footer__logo{
  width: 40px;
  height: 40px;
  margin: 20px;
}
.footer__logo:hover{
  cursor: pointer;
}
</style>