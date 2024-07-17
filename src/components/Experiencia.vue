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
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam suscipit auctor efficitur. 
                Morbi gravida dui vel ligula gravida rutrum. Morbi.
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

