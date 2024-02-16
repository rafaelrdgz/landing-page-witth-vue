<script setup>

</script>

<template>
  <header class="header">
    <img class="header__logo" src="https://cdn.freecodecamp.org/testable-projects-fcc/images/product-landing-page-logo.png" alt="Company Logo">
    <nav class="header__nav">
      <ul class="nav__list">
        <li><a href="">Features</a></li>
        <li><a href="">How it works</a></li>
        <li><a href="">Pricing</a></li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
.header{
  width: 100%;
  height: 80px;
  background-color: #f4a261;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.header__logo{
  height: 40px;
}
.nav__list{
  display: flex;
  justify-content: space-around;
  width: 400px;
}
.nav__list li{
  list-style: none;
}
.nav__list li a{
  text-decoration: none;
  color: black;
  font-size: 25px;
}
@media (320px <= width <= 768px) {
  .header__logo{
    width: 300px;
  }
}
</style>