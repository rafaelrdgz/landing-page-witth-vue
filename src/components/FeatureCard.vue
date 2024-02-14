<script setup>
const props = defineProps(['featureImg', 'featureTitle', 'featureDescription'])

</script>

<template>
  <section class="container">
    <div class="img-container">
      <img src="../assets/truck.png" alt="" >
    </div>
    <div class="description-container">
      <h3 class="feature-title">{{featureTitle}}</h3>
      <p class="feature-description">{{featureDescription}}</p>
    </div>
  </section>
</template>

<style scoped>
.container{
  display: flex;
  align-items: center;
  margin: 0 200px -30px 200px;
}
.img-container img{
  width: 200px;
}
.feature-title{
  font-size: 30px;
  margin-bottom: -10px;
}
.feature-description{
  font-size: 18px;
}
</style>