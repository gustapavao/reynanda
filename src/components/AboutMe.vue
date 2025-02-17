<script setup>

</script>

<template>
  <div id="about-me-box">
    <div id="about-me-content">
    <p>
      Sou de Ananindeua - PA, amo a minha culinária paraense, mas
      meu coração é intensamente Maranhense e sou apaixonada por
      essa cultura cheia de história.
    </p>
    <p>
      Comecei a trabalhar como modelo fotográfica em 2019, com
      ensaios artísticos ( e sou completamente apaixonada por essa arte)
      e desde então o amor pela fotografia só aumentou. Logo em
      seguida, perdi a vergonha (que já era pouca mesmo) e comecei a
      gravar conteúdo para o Instagram, na caminhada eu fui
      descobrindo novas paixões, como edição de vídeos e todo o meio
      virtual.
    </p>
    <p>
      Me sinto muito a vontade na frente de uma câmera, seja para tirar
      fotos ou falar com telespectadores, uso as minhas redes sociais
      para me expressar e motivar pessoas. Trabalhei em campanhas
      para a Equatorial, Dal Cotone Italy, Aestimare, Kukáh, NIT Fitwear.
    </p>
    <p>
      Atualmente, meus nichos principais são lifestyle, moda e o mundo
      fitness. Não trabalho com marcas da qual eu não acredito, divulgo
      o que eu uso e gosto, e espero que juntos possamos alcançar
      muitas pessoas dispostas a abraçar o nosso trabalho!!!!
    </p>
  </div>
    <img src="@/assets/about-me-photo.png">
    <h3>Sobre Mim</h3>
  </div>
</template>

<style scoped>
  #about-me-box{
    margin-top: 8rem;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
  }
  #about-me-content{
    margin-top: 2rem;
    max-width: 50%;
    font-size: 1.6rem;
    margin-right: 1.6rem;
    font-family: 'Lora', serif;
  }
  h3{
    font-family: "Times New Roman", serif;
    position: absolute;
    transform: rotate(-90deg);
    left: 96rem;
    top: 92rem;
    font-size: 80px;
    font-weight: lighter;
    white-space: nowrap;
  }
  p{
    margin-bottom: 0.8rem;
  }
  img{
    width: 679px;
  }
</style>