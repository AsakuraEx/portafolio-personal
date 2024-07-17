<script setup>
  import {ref, reactive, onMounted} from 'vue';
  
  import Header from './components/Header.vue';
  import Habilidades from './components/Habilidades.vue';
  import Experiencia from './components/Experiencia.vue';
  import Contactame from './components/Contactame.vue';
  import { db1 } from './data/habilidades';
  import { db2 } from './data/experiencia';

  const habilidades = ref([]);
  const experiencias = ref([]);

  onMounted(()=>{
      habilidades.value = db1;
      experiencias.value = db2;
  })

  

</script>

<template>
  
  <div class="container mx-auto">
    <Header />

    <Habilidades 
      :habilidades="habilidades"
    />

    <Experiencia 
      :experiencias="experiencias"
    />

    <Contactame />

    <div class="text-center md:flex md:justify-between mt-4 items-center text-white border-t border-slate-200 pt-12">
      <h1 class="text-3xl font-bold mb-5 md:mb-0 text-green-500">

          Francisco Escobar
      </h1>
      <ul class="flex gap-4 flex-col md:flex-row">
          <li class="text-lg cursor-pointer hover:text-slate-200"><a href="#">Quién Soy</a></li>
          <li class="text-lg cursor-pointer hover:text-slate-200"><a href="#habilidades">Habilidades</a></li>
          <li class="text-lg cursor-pointer hover:text-slate-200"><a href="#experiencia">Experiencia</a></li>
          <li class="text-lg cursor-pointer hover:text-slate-200"><a href="#contactame">Contactame</a></li>
      </ul>
    </div>

    <footer class="px-8 py-12 text-white text-lg text-center">
        &copy; Francisco Josue Escobar Quintanilla
    </footer>
  </div>

</template>

