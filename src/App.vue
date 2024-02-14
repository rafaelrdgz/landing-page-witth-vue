<script setup>
import Header from "./components/Header.vue";
import FeatureCard from "./components/FeatureCard.vue";
import TruckImg from './assets/truck.png'

defineProps({
  featureImg: String,
  featureTitle: String,
  featureDescription: String
})
</script>

<template>
  <Header></Header>
  <h1 class="title">Handcrafted, home-made masterpieces</h1>
  <form class="form">
    <input class="form__email" type="text" name="" id="" placeholder="Enter your email address" required>
    <button class="submit-btn" type="submit">Get Started</button>
  </form>
  <section id="features">
    <FeatureCard
        feature-img=""
        feature-description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi aperiam asperiores aut, consequatur doloremque dolorum ea enim exercitationem inventore iure, minus nam neque nesciunt officia ullam, ut veritatis voluptas voluptates."
        feature-title="Fast Shipping"></FeatureCard>
  </section>



</template>

<style scoped>
.title{
  text-align: center;
  margin-top: 40px;
  font-size: 40px;
}
.form{
  display: flex;
  justify-content: center;
  margin-bottom: 50px;
}
.form__email{
  height: 40px;
  border: none;
  border-radius: 5px;
  padding-left: 20px;
  width: 220px;
  font-size: 15px;
}
.submit-btn{
  background: #f4a261;
  border: none;
  border-radius: 5px;
  font-size: 20px;
  font-weight: bold;
}
</style>
