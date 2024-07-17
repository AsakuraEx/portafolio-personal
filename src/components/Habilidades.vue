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
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam suscipit auctor efficitur. 
            Morbi gravida dui vel ligula gravida rutrum. Morbi.
        </p>
    </div>

    <div 
        class="grid grid-cols-1 md:grid-cols-3 my-10 px-8 gap-4"
    >
        
        <div v-for="habilidad in habilidades" class="flex flex-col justify-center items-center gap-6 py-12 bg-slate-100 rounded-md">
            <h3 class="text-center text-green-600 text-2xl font-bold uppercase">{{ habilidad.nombre }}</h3>
            <img :src="habilidad.imagen" alt="Logo Tailwind" class="w-52">
            <h3 class="text-center text-orange-600 text-5xl font-black uppercase">{{ habilidad.porcentaje }}</h3>
            <p class="text-black px-8 italic">
                {{ habilidad.descripcion }}
            </p>
        </div>
        
    </div>
</template>