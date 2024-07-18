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
            <li class="text-lg cursor-pointer hover:text-slate-200"><a href="#proyectos">Proyectos</a></li>
            <li class="text-lg cursor-pointer hover:text-slate-200"><a href="#contactame">Contactame</a></li>
        </ul>
    </div>

    <div class="flex flex-col-reverse md:flex-row gap-8 mt-20 justify-center items-center">
        <article class="text-white md:px-0 md:w-1/2 px-8 space-y-4">
                <h2 class="font-bold text-3xl text-center text-green-500 uppercase">Acerca de mi</h2>
                <p class="text-justify">
                    Mi nombre es Francisco Josue Escobar Quintanilla, tengo 27 años en pleno 2024 y resido en el departamento de San Salvador en El Salvador me encanta la informática, los juegos de video y la cultura japonesa; entre mis pasatiempo estan los videojuegos y 
                    la busqueda de conocimiento informático, soy una persona amigable, con muy buenas relaciones personales, proactivo y que le gusta apoyar en los trabajos de equipo, 
                    siendo agil en el desarrollo de labores.
                    <br><br>
                    Una de las areas de la informática que me apasionan es el area de desarrollo, mi area destacada es el analisis y diseño de sistemas, pero además me encanta el hardware; 
                    poder probar componentes, armar equipos y realizar pruebas de rendimiento y funcionalidad de equipos, realizar ensambles de equipos optimizados para propositos especificos.
                    <br><br>
                    Soy jugador activo de PC, juego mediante plataformas como Steam o Epic, además me gusta ver algún anime de temporada y buscar el conocimiento técnico sobre diferentes intereses 
                    con respecto a la informática.
                    <br><br>
                    Si he captado tu atención, puedes seguir leyendo mi portafolio, seguro que te puede interesar. 
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