<script setup>

</script>

<template>
  <div class="spacing"></div>
  <div id="medidas">
    <h3>Medidas</h3>
    <div class="lists-container">
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
    </div>
    <img src="@/assets/medidas.png" alt="">
  </div>
</template>

<style scoped>
.spacing {
  margin: 10rem 0;
}

h3 {
  font-family: 'Raleway', sans-serif;
  transform: rotate(-90deg);
  font-size: 6vw;
  font-weight: lighter;
}

#medidas {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  gap: 3rem;
  flex-wrap: wrap; /* Permite que os elementos se ajustem em telas menores */
}

.lists-container {
  display: flex;
  flex-direction: row;
  gap: 3rem;
}

.list-group {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  text-align: right;
}

.list-group li {
  font-weight: 800;
  font-size: 2rem;
}

ul {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  text-align: left;
}

ul li {
  font-size: 2rem;
  list-style-type: none;
}

img {
  width: 100%;
  max-width: 400px;
  height: auto;
  margin-top: 1.5rem; /* Espaço para a imagem */
}

/* Media queries para ajustar os tamanhos */
@media (max-width: 1024px) {
  #medidas {
    gap: 2rem;
  }

  h3 {
    transform: rotate(0);
    font-size: 5vw;
  }

  .list-group li,
  ul li {
    font-size: 1.8rem;
  }

  img {
    max-width: 350px;
  }
}

@media (max-width: 768px) {
  #medidas {
    flex-direction: column; /* Muda para coluna para telas menores */
    gap: 1.5rem;
  }

  h3 {
    font-size: 5.5vw;
  }

  .list-group li,
  ul li {
    font-size: 1.6rem;
  }

  img {
    max-width: 300px;
  }
}

@media (max-width: 480px) {
  #medidas {
    flex-direction: column; /* Garante que continue em coluna em telas muito pequenas */
    gap: 1rem;
  }

  h3 {
    font-size: 6vw;
  }

  .list-group li,
  ul li {
    font-size: 1.4rem;
  }

  img {
    max-width: 250px;
  }
}
</style>
