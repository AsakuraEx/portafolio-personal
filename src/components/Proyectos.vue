<script setup>
    const props = defineProps({
        proyectos: {
            type: Array,
            required: true
        }
    })
</script>

<template>
    <div class="space-y-8 mt-10">
        <div class="flex flex-col gap-8 text-center" id="proyectos">
            <h1 class="text-green-500 text-3xl font-bold uppercase">Proyectos</h1>
            <p class="text-justify md:text-center text-lg text-white px-8">
                En este apartado te muestro algunos de los proyectos que he realizado, algunos proyectos son realizados como practica para 
                utilizar diferentes tecnologías y descubrir nuevas formas de implementarlas y otros proyectos son proyectos desarrollados para
                pequeñas empresas.
                <br><br>
                <center><b class="uppercase">Da clic en el nombre de cada proyecto para visualizarlo</b></center>
            </p>
        </div>
    
        <div class="mx-8 grid grid-flow-row gap-2">
            <div 
                class="bg-slate-100 p-8 rounded-md flex flex-col items-center md:flex-row gap-8"
                v-for="proyecto in proyectos"    
            >
                <img src="/img/star.svg" alt="estrella" class="w-12">
                <div class="flex flex-col w-full md:justify-center">
                    <h3 class="font-bold text-2xl text-center hover:text-green-500">
                        <a :href="proyecto.url" target="_blank">
                            {{ proyecto.titulo }}
                        </a>
                    </h3>
                    <p class="text-justify mx-auto text-xl">
                        {{ proyecto.descripcion }}
                    </p>
                </div>
            </div>

        </div>
    </div>
</template>