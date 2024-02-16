<script setup>
import Header from "./components/Header.vue";
import FeatureCard from "./components/FeatureCard.vue";
import PriceCard from "./components/PriceCard.vue";
import Footer from "./components/Footer.vue";

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
  <section id="features-container">
    <FeatureCard
        feature-img=""
        feature-description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi aperiam asperiores aut, consequatur doloremque dolorum ea enim exercitationem inventore iure, minus nam neque nesciunt officia ullam, ut veritatis voluptas voluptates."
        feature-title="Fast Shipping">
    </FeatureCard>
    <FeatureCard
        feature-img=""
        feature-description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi aperiam asperiores aut, consequatur doloremque dolorum ea enim exercitationem inventore iure, minus nam neque nesciunt officia ullam, ut veritatis voluptas voluptates."
        feature-title="Fast Shipping">
    </FeatureCard>
    <FeatureCard
        feature-img=""
        feature-description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi aperiam asperiores aut, consequatur doloremque dolorum ea enim exercitationem inventore iure, minus nam neque nesciunt officia ullam, ut veritatis voluptas voluptates."
        feature-title="Fast Shipping">
    </FeatureCard>
  </section>
  <section id="pricing-container">
    <PriceCard></PriceCard>
    <PriceCard></PriceCard>
    <PriceCard></PriceCard>
  </section>
  <Footer></Footer>



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
  cursor: pointer;
}
#features-container{
  margin: 0 100px;
}
#pricing-container{
  display: flex;
  justify-content: space-between;
  margin: 80px 400px;
}
@media (width <= 425px) {
  #features-container{
    margin: 0;
  }
  .form{
    margin-bottom: 0;
  }
  #pricing-container{
    flex-wrap: wrap;
    justify-content: center;
    margin: 40px 50px;
  }
}
@media (425px < width <= 768px) {
  #pricing-container{
    flex-wrap: wrap;
    justify-content: center;
    margin: 40px 120px;
  }
}
@media ( 768px < width < 1024px ) {
  #pricing-container{
    margin: 50px 80px;
  }
}
@media ( 1024px <= width <= 1440px ) {
  #pricing-container{
    margin: 50px 60px;
    justify-content: space-around;
  }
}
</style>
