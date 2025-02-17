<script setup>
//const openReadmeInEditor = () => fetch('/__open-in-editor?file=README.md')
</script>

<template>
  <div id="welcome-box">
    <div id="text-welcome">
      <h4>Portfólio de Modelo</h4>
      <h1>Reynanda</h1>
      <h1>Rocha</h1>
      <button>Entre em contato comigo</button>
    </div>
    <img src="@/assets/welcome-photo.png" alt="Foto de boas-vindas">
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
