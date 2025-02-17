<script setup>

</script>

<template>
  <button>Entre em contato comigo</button>
  <div id="spacing"></div>
</template>

<style scoped>

#spacing {
  margin-top: 3rem;
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
  margin: auto;
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

@media (max-width: 768px) {
  button {
    margin-top: 3rem;
  }

  @media (max-width: 480px) {
    button {
      width: auto;
      max-width: 80%;
      font-size: 1rem;
      margin-bottom: 2rem;
      margin-left: 1rem;
    }
  }}
</style>