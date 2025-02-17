<script setup>

</script>

<template>
<div class="spacing"></div>
  <div id="medidas">
    <h3>
      Medidas
    </h3>
    <ul class="list-group">
      <li>Altura</li>
      <li>Busto</li>
      <li>Cintura</li>
      <li>Quadril</li>
      <li>Sapatos</li>
      <li>Tamanho</li>
      <li>Cabelo</li>
      <li>Olhos</li>
    </ul>
    <ul>
      <li>1,57</li>
      <li>81</li>
      <li>66</li>
      <li>95</li>
      <li>35</li>
      <li>PP/P</li>
      <li>Ruivo</li>
      <li>Castanhos Escuro</li>
    </ul>
    <img src="@/assets/medidas.png" alt="">
  </div>
</template>

<style scoped>
.spacing {
  margin: 10rem 0;
}

h3{
  font-family: 'Raleway', sans-serif;
  transform: rotate(-90deg);
  font-size: 80px;
  font-weight: lighter;
}

#medidas{
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.list-group li {
  font-weight: 800;
  margin-left: 10rem;
}

li {
  list-style-type: none;
  font-size: 2.4rem;
  margin-right: 2.4rem;
}
</style>