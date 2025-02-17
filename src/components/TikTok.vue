<script setup>

</script>

<template>
  <div class="spacing"></div>
  <div class="instagram">
    <h3>Alcance:</h3>
    <h3>TikTok</h3>
    <img src="@/assets/tiktok-1.png" alt="">
    <img src="@/assets/tiktok-2.png" alt="">
    <img src="@/assets/tiktok-3.png" alt="">
  </div>
  <div class="spacing"></div>
</template>

<style scoped>
.spacing {
  margin: 10rem 0;
}

.instagram {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

h3{
  font-family: 'Raleway', sans-serif;
  transform: rotate(-90deg);
  font-size: 80px;
  font-weight: lighter;
  margin-left: -11rem;
}



img{
  margin-right: 1.6rem;
}


</style>
