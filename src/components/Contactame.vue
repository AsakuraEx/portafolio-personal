<script setup>

</script>

<template>
    <div class="mt-10 mx-8 bg-green-700 rounded py-12">
        <h1 class="text-white font-bold text-3xl text-center mb-12 uppercase">Contactame</h1>
        <div class="flex flex-col gap-12 md:flex-row-reverse">
            <form
                class="mx-8 px-8  md:w-1/2"
            >
                <div class="space-y-4">
                    <div class="flex flex-col gap-3">
                        <label 
                            for="nombre"
                            class="text-white font-semibold"
                        >
                            Ingresa tu nombre:
                        </label>
                        <input 
                            class="border p-2 rounded"
                            type="text" 
                            id="nombre" 
                            placeholder="Escribe tu nombre aqui"
                        >
                    </div>
                    <div class="flex flex-col gap-3">
                        <label 
                            for="telefono"
                            class="text-white font-semibold"
                        >
                            Telefono:
                        </label>
                        <input 
                            type="text" 
                            id="telefono" 
                            placeholder="Ingresa tu numero de contacto"
                            class="border p-2 rounded"
                        >
                    </div>
                    <div class="flex flex-col gap-3">
                        <label 
                            for="email"
                            class="text-white font-semibold"
                        >
                            Correo electronico:
                        </label>
                        <input 
                            type="email" 
                            id="email" 
                            placeholder="Ingresa tu correo electronico"
                            class="border p-2 rounded"
                        >
                    </div>
                    <div>
                        <button
                            class="bg-orange-700 p-3 w-full text-white uppercase font-bold rounded-md
                            hover:bg-orange-800"
                        >
                            Enviar Datos de Contacto
                        </button>
                    </div>
                </div>

                
                


            </form>
            <picture class="md:w-1/2 flex justify-center items-center">
                <img 
                    src="/img/contact-us.svg" 
                    alt="Imagen de contacto"
                    class="h-72 px-8"
                >
            </picture>
        </div>
    </div>
</template>
