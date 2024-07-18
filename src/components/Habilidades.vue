<script setup>
    const props = defineProps({
        habilidades: {
            type: Array,
            required: true
        }
    })
</script>

<template>
    <div class="text-white px-8 mt-20 space-y-4" id="habilidades">
        <h1 class="text-3xl font-bold text-center text-green-500 uppercase">Habilidades</h1>
        <p class="text-justify md:text-center text-lg">
            Entre las habilidades más destacadas son el mantenimiento de hardware y software, el análisis y diseño de aplicaciones web y el manejo de base de datos; en 
            el caso del desarrollo, me interesa mucho el desarrollo web aspirando a convertirme en un desarrollador full stack, he practicado algunas tecnologías para front-end y back-end.
            <br><br>
            Entre las tecnologías que he utilizado, te listo las que más son de mi interes en el desarrollo de aplicaciones web.
        </p>
    </div>

    <div 
        class="grid grid-cols-1 md:grid-cols-3 my-10 px-8 gap-4"
    >
        
        <div v-for="habilidad in habilidades" class="flex flex-col justify-center items-center gap-6 py-12 bg-slate-100 rounded-md">
            <h3 class="text-center text-green-600 text-2xl font-bold uppercase">{{ habilidad.nombre }}</h3>
            <img :src="habilidad.imagen" alt="Logo Tailwind" class="w-48">
            <h3 class="text-center text-orange-600 text-5xl font-black uppercase">{{ habilidad.porcentaje }}</h3>
            <p class="text-black px-8 italic">
                {{ habilidad.descripcion }}
            </p>
        </div>
        
    </div>
</template>