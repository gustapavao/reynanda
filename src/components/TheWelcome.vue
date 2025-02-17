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
    <img src="@/assets/welcome-photo.png">
  </div>
</template>

<style scoped>
  #welcome-box{
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
  }

  h4{
    font-size: 1rem;
    margin-left: 4rem;
    margin-bottom: 4rem;
  }

  h1{
    font-size: 12rem;
    margin-bottom: -8rem;
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
                                                       font-family: ui-sans-serif,system-ui,-apple-system,system-ui,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";
                                                       font-size: 1rem;
                                                       font-weight: 700;
                                                       justify-content: center;
                                                       line-height: 1.75rem;
                                                       padding: .75rem 1.65rem;
                                                       position: relative;
                                                       text-align: center;
                                                       text-decoration: none #000000 solid;
                                                       text-decoration-thickness: auto;
                                                       width: 100%;
                                                       max-width: 460px;
                                                       position: relative;
                                                       cursor: pointer;
                                                       transform: rotate(-2deg);
                                                       user-select: none;
                                                       -webkit-user-select: none;
                                                       touch-action: manipulation;
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

  @media (min-width: 768px) {
    button {
      padding: .75rem 3rem;
      font-size: 1.25rem;
    }
  }
</style>
