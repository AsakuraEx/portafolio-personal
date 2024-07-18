<script setup>
    const props = defineProps({
        experiencias: {
            type: Array,
            required: true
        }
    })
</script>

<template>
    <div class="space-y-8">
        <div class="flex flex-col gap-8 text-center" id="experiencia">
            <h1 class="text-green-500 text-3xl font-bold uppercase">Experiencia</h1>
            <p class="text-justify md:text-center text-lg text-white px-8">
                A lo largo del tiempo he desempeñado mi profesión de distintas maneras, inicialmente en mi infancia vendia juegos que eran descargados de internet y posteriormente almacenados en CDs o DVDs;
                posterior a recibir una formación de informática en mi Bachillerato, lograba realizar trabajos de mantenimiento correctivo y preventivo a equipos de familiares, conocidos y algunas personas que
                llegaban a mi por recomendación.
                <br><br>
                Finalmente logre ganar experiencia en diferentes empresas e instituciones en las que se me ha permitido laborar, te las listo a continuación, indicandote en una breve descripción algunas funciones que ejercía
                en cada una de las empresas e instituciones
            </p>
        </div>
    
        <div class="mx-8 grid grid-flow-row gap-2">
            <div 
                class="bg-slate-100 p-8 rounded-md flex flex-col items-center md:flex-row gap-8"
                v-for="experiencia in experiencias"    
            >
                <img src="/img/star.svg" alt="estrella" class="w-12">
                <div class="flex flex-col w-full md:justify-center">
                    <h3 class="font-bold text-2xl text-center">{{ experiencia.titulo }}</h3>
                    <h4 class="font-light text-md text-center">{{ experiencia.fecha }}</h4>
                    <p class="text-justify mx-auto text-xl">
                        {{ experiencia.descripcion }}
                    </p>
                </div>
            </div>

        </div>
    </div>

</template>

