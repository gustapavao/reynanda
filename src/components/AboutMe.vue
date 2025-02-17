<script setup>

</script>

<template>
  <div id="about-me-box">
    <div id="about-me-content">
      <h3>Sobre Mim</h3>
      <p>
        Sou de Ananindeua - PA, amo a minha culinária paraense, mas
        meu coração é intensamente Maranhense e sou apaixonada por
        essa cultura cheia de história.
      </p>
      <p>
        Comecei a trabalhar como modelo fotográfica em 2019, com
        ensaios artísticos (e sou completamente apaixonada por essa arte)
        e desde então o amor pela fotografia só aumentou. Logo em
        seguida, perdi a vergonha (que já era pouca mesmo) e comecei a
        gravar conteúdo para o Instagram. Na caminhada, fui
        descobrindo novas paixões, como edição de vídeos e todo o meio
        virtual.
      </p>
      <p>
        Me sinto muito à vontade na frente de uma câmera, seja para tirar
        fotos ou falar com telespectadores. Uso as minhas redes sociais
        para me expressar e motivar pessoas. Trabalhei em campanhas
        para a Equatorial, Dal Cotone Italy, Aestimare, Kukáh, NIT Fitwear.
      </p>
      <p>
        Atualmente, meus nichos principais são lifestyle, moda e o mundo
        fitness. Não trabalho com marcas das quais eu não acredito, divulgo
        o que uso e gosto, e espero que juntos possamos alcançar
        muitas pessoas dispostas a abraçar o nosso trabalho!!!!
      </p>
    </div>
<!--    <img src="@/assets/about-me-photo.png" alt="Foto sobre mim">-->
  </div>
</template>

<style scoped>
#about-me-box {
  margin-top: 8rem;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  text-align: center;
}

#about-me-content {
  margin-top: 2rem;
  max-width: 50%;
  font-size: 1.6rem;
  margin-right: 1.6rem;
  font-family: 'Lora', serif;
}

h3 {
  font-family: 'Raleway', sans-serif;
  font-size: clamp(2rem, 5vw, 80px);
  font-weight: lighter;
  white-space: nowrap;
  position: relative;
  transform: none;
  left: auto;
  top: auto;
  margin-top: 2rem;
}

p {
  margin-bottom: 0.8rem;
}

img {
  width: 100%;
  max-width: 679px;
  height: auto;
}

@media (max-width: 768px) {
  #about-me-box {
    flex-direction: column;
    align-items: center;
  }

  #about-me-content {
    max-width: 90%;
    font-size: 1.4rem;
    margin-right: 0;
  }

  h3 {
    font-size: 3rem;
    margin-top: 1rem;
  }
}
</style>