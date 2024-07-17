<script setup>

</script>

<template>
    
    <div class="text-center md:flex md:justify-between mt-4 items-center text-white">
        <h1 class="text-3xl font-bold mb-5 md:mb-0 text-green-500">
            <span class="text-white block">Portafolio</span>
            Francisco Escobar
        </h1>
        <ul class="flex gap-4 flex-col md:flex-row">
            <li class="text-lg cursor-pointer hover:text-slate-200"><a href="#">Quién Soy</a></li>
            <li class="text-lg cursor-pointer hover:text-slate-200"><a href="#habilidades">Habilidades</a></li>
            <li class="text-lg cursor-pointer hover:text-slate-200"><a href="#experiencia">Experiencia</a></li>
            <li class="text-lg cursor-pointer hover:text-slate-200"><a href="#contactame">Contactame</a></li>
        </ul>
    </div>

    <div class="flex flex-col-reverse md:flex-row gap-8 mt-20 justify-center items-center">
        <article class="text-white md:px-0 md:w-1/2 px-8 space-y-4">
                <h2 class="font-bold text-3xl text-center text-green-500 uppercase">Acerca de mi</h2>
                <p class="text-justify">
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam suscipit auctor
                     efficitur. Morbi gravida dui vel ligula gravida rutrum. Morbi.
                </p>
        </article>
        
        <picture class="md:w-1/2 items-center justify-center">
            <img 
                class="w-64 md:w-72 aspect-square rounded-full mx-auto"
                src="/img/Cat03.jpg" 
                alt="Foto de perfil"
            />
        </picture>
    </div>
    
</template>