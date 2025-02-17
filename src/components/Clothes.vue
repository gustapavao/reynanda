<script setup>

</script>

<template>
  <div class="spacing"></div>
  <div class="clothes">
    <h3>
      Vestuário
    </h3>
    <img id="img1" src="@/assets/vestuario-1.png" alt="">
    <img id="img2" src="@/assets/vestuario-2.png" alt="">
    <img id="img3" src="@/assets/vestuario-1.png" alt="">
  </div>


</template>

<style scoped>
.spacing {
  margin: 10rem 0;
}

.clothes {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

h3{
  font-family: "Times New Roman", serif;
  transform: rotate(-90deg);
  font-size: 80px;
  font-weight: lighter;
}

img{
  height: auto;
  width: auto;
}

#img1{
  margin-left: -2rem;
  padding-bottom: 8rem;
  margin-right: 4px;
}

#img2{
  padding-top: 8rem;
}

#img3 {
  padding-bottom: 8rem;
  margin-right: 4px;
}
</style>