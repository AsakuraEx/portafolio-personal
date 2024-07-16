<script setup>
  import Header from "./components/Header.vue";
  import Habilidades from "./components/Habilidades.vue";
  import Experiencia from "./components/Experiencia.vue";
  import Contactame from "./components/Contactame.vue";
</script>

<template>
  
  <div class="container mx-auto">
    <Header />

    <Habilidades />

    <Experiencia />

    <Contactame />

    <footer class="px-8 py-12 text-white text-lg text-center">
        &copy; Francisco Josue Escobar Quintanilla
    </footer>
  </div>

</template>

