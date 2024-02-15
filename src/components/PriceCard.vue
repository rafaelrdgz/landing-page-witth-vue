<script setup>

</script>

<template>
  <div class="price-card">
    <h3 class="card-title">Basic</h3>
    <h3 class="card-price">$600/month</h3>
    <ul>
      <li>Plays similar to a Trumpet</li>
      <li>Plays similar to a Trumpet</li>
      <li>Plays similar to a Trumpet</li>
    </ul>
    <button class="select-btn">Select</button>
  </div>
</template>

<style scoped>
.price-card {
  border: solid #f4a261;
  border-radius: 10px;
  text-align: center;
  width: 270px;
  height: 300px;
}
.price-card:hover{
  box-shadow: 5px 0 40px rgba(0,0,0, .2);
}
.card-title{
  background: #f4a261;
  margin: 0;
  padding: 20px;
  font-size: 25px;
}
.card-price{
  font-size: 22px;
}
.price-card ul{
  list-style: none;
  padding: 0;
}
.price-card li{
  padding-top: 10px;
}
.select-btn{
  background: #f4a261;
  width: 80px;
  height: 40px;
  border: none  ;
  border-radius: 5px;
  font-size: 20px;
  font-weight: bold;
}
.select-btn:hover{
  box-shadow: 5px 0 40px rgba(0,0,0, .2);
}
@media (425px <= width <= 768px) {
  .price-card{
    margin-bottom: 30px;
  }
}
</style>