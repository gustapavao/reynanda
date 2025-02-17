<script setup>

</script>

<template>
  <div class="spacing"></div>
  <div class="instagram">
    <h3>Alcance: Instagram</h3>
    <img src="@/assets/alcance-insta-1.png" alt="">
    <img src="@/assets/alcance-insta-2.png" alt="">
  </div>
</template>

<style scoped>
.spacing {
  margin: 10rem 0;
}

.instagram {
  display: flex;
  flex-direction: row; /* Padrão: elementos dispostos em linha */
  justify-content: center;
  align-items: center;
  gap: 2rem;
}

h3 {
  font-family: 'Raleway', sans-serif;
  font-size: 6vw;
  font-weight: lighter;
}

img {
  margin-right: 1.6rem;
  width: 100%;
  max-width: 300px; /* Limite o tamanho da imagem */
  height: auto;
}

/* Media queries para telas menores */
@media (max-width: 1024px) {
  .instagram {
    gap: 1.5rem;
  }

  h3 {
    font-size: 5vw;
  }

  img {
    max-width: 250px;
  }
}

@media (max-width: 768px) {
  .instagram {
    flex-direction: column; /* Altera para coluna em telas menores */
    gap: 1rem;
  }

  h3 {
    font-size: 5vw;
  }

  img {
    max-width: 200px;
  }
}

@media (max-width: 480px) {
  .instagram {
    flex-direction: column; /* Garante que ainda esteja em coluna nas telas pequenas */
    gap: 0.8rem;
  }

  h3 {
    font-size: 6vw;
    margin-left: 0; /* Ajuste do margin-left para evitar deslocamento */
  }

  img {
    max-width: 150px;
  }
}
</style>
