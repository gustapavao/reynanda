<script setup>
import { ref } from 'vue';

const showPopup = ref(false);
const email = 'reynandarch@gmail.com';

const openEmailClient = () => {
  window.location.href = `mailto:${email}`;
};

const copyEmail = () => {
  navigator.clipboard.writeText(email).then(() => {
    alert('E-mail copiado para a área de transferência!');
  });
};
</script>

<template>
  <div id="welcome-box">
    <div id="text-welcome">
      <h4>Portfólio de Modelo</h4>
      <h1>Reynanda</h1>
      <h1>Rocha</h1>
      <button @click="showPopup = true">Entre em contato comigo</button>
    </div>
    <img src="@/assets/welcome-photo.png" alt="Foto de boas-vindas">
  </div>

  <!-- Pop-up -->
  <div v-if="showPopup" class="popup-overlay">
    <div class="popup">
      <p>Meu e-mail: {{ email }}</p>
      <div class="popup-buttons">
        <button @click="openEmailClient">Abrir E-mail</button>
        <button @click="copyEmail">Copiar E-mail</button>
      </div>
      <button @click="showPopup = false" class="close-popup">Fechar</button>
    </div>
  </div>
</template>

<style scoped>
#welcome-box {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  text-align: center;
}

h4 {
  font-size: 1rem;
  margin-left: 4rem;
  margin-bottom: 4rem;
}

h1 {
  font-size: clamp(3rem, 10vw, 12rem);
  margin-bottom: -4rem;
  font-family: "Times New Roman", serif;
  font-weight: 100;
  margin-right: 1rem;
}

button {
  margin-top: 10rem;
  background-color: #737373;
  border: 0 solid #E5E7EB;
  box-sizing: border-box;
  color: #000000;
  display: flex;
  font-family: ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 1rem;
  font-weight: 700;
  justify-content: center;
  line-height: 1.75rem;
  padding: .75rem 1.65rem;
  position: relative;
  text-align: center;
  text-decoration: none;
  width: auto;
  max-width: 460px;
  cursor: pointer;
  transform: rotate(-2deg);
  user-select: none;
  margin-bottom: 1rem;
}

button:focus {
  outline: 0;
}

button:after {
  content: '';
  position: absolute;
  border: 1px solid #000000;
  bottom: 4px;
  left: 4px;
  width: calc(100% - 1px);
  height: calc(100% - 1px);
}

button:hover:after {
  bottom: 2px;
  left: 2px;
}

img {
  max-width: 100%;
  height: auto;
}

/* Estilo do Pop-up */
.popup-overlay {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 9999;
}

.popup {
  background-color: #fff;
  padding: 2rem;
  border-radius: 8px;
  width: 80%;
  max-width: 400px;
  text-align: center;
}

.popup-buttons {
  margin-top: 1rem;
}

.popup-buttons button {
  background-color: #4CAF50;
  color: white;
  padding: 0.75rem 1.5rem;
  margin: 0.5rem;
  border: none;
  cursor: pointer;
  border-radius: 5px;
}

.popup-buttons button:hover {
  background-color: #45a049;
}

.close-popup {
  background-color: #f44336;
  color: white;
  padding: 0.75rem 1.5rem;
  margin-top: 1rem;
  border: none;
  cursor: pointer;
  border-radius: 5px;
}

.close-popup:hover {
  background-color: #e60000;
}

@media (max-width: 768px) {
  #welcome-box {
    flex-direction: column;
    align-items: center;
  }

  h4 {
    margin-left: 0;
    margin-bottom: 2rem;
  }

  h1 {
    font-size: 4rem;
    margin-bottom: 30rem;
  }

  button {
    margin-top: 3rem;
  }

  img {
    width: 80%;
    max-width: 300px;
  }
}

@media (max-width: 480px) {
  button {
    width: auto;
    max-width: 80%;
    font-size: 1rem;
    margin-bottom: 2rem;
    margin-left: 1rem;
  }

  h1 {
    font-size: 4rem;
    margin-bottom: -2rem;
  }
}
</style>
