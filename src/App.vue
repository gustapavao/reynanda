<script setup>
import { RouterLink, RouterView } from 'vue-router'
import TheWelcome from './components/TheWelcome.vue'
import AboutMe from "./components/AboutMe.vue";
import Clothes from "./components/Clothes.vue";
import Medidas from "@/components/Medidas.vue";
import Instagram from "@/components/Instagram.vue";
import TikTok from "@/components/TikTok.vue";
import ContrateMe from "@/components/Contrate-me.vue";

</script>

<template>
  <header>
<!--    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />-->
    <TheWelcome></TheWelcome>
    <AboutMe></AboutMe>
    <Clothes></Clothes>
    <Medidas></Medidas>
    <Instagram></Instagram>
    <TikTok></TikTok>
    <ContrateMe></ContrateMe>

<!--    <div class="wrapper">-->
<!--      <nav>-->
<!--        <RouterLink to="/">Home</RouterLink>-->
<!--        <RouterLink to="/about">About</RouterLink>-->
<!--      </nav>-->
<!--    </div>-->
  </header>

  <RouterView />
</template>

