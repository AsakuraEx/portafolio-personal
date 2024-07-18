<script setup>
    
    import {computed} from 'vue';
    const props = defineProps(
        {
            alerta:{
                type: Object,
                required:true
            }
        }
    );

    const isError = computed(()=>{
        return props.alerta.tipo === 'error';
    })
</script>

<template>
    <div
        :class="[isError ? 'bg-red-600':'bg-blue-600']" 
        class="mt-10 mx-8 px-8 py-4 text-center bg-red-600 rounded">
        <p class="text-white font-bold uppercase">{{ alerta.mensaje }}</p>
    </div>
</template>
