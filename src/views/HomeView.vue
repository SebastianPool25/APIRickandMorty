<script setup>
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <body class="bg-green-500">
    <div class="grid grid-cols-2 gap-2">

      <div class="p-7 mx-5 my-5 font-mono">
        <h1 class="text-4xl font-bold">Rick and Morty</h1>
        <br>
        <h2 class="text-xl font-semibold">Sinopsis:</h2>
        <p class="text-lg pr-8">
          Después de haber estado desaparecido durante casi 20 años, Rick Sánchez llega de imprevisto a la puerta de la casa de su hija Beth y se va a vivir con ella y su familia utilizando el garaje como su laboratorio personal.
        </p>
        <br>
        <h2 class="text-xl font-semibold">Creadores:</h2>
        <p class="text-lg pr-8">
          Justin Roiland y Dan Harmon
        </p>
        <br>
        <h2 class="text-xl font-semibold">Número de temporadas:</h2>
        <p class="text-lg pr-8">6</p>
        <br>
        <h2 class="text-xl font-semibold">Número de capítulos</h2>
        <p class="text-lg pr-8">61</p>
        <br>
        <h2 class="text-xl font-semibold">Disponible en:</h2>
        <a href="https://www.hbomax.com/mx/es">HBO Max</a>

      </div>

      <div class="contenedor p-7 mx-10">
        <img src="../assets/posterjpg.jpg" alt="PosterRickAndMorty" height="200" width="460" class="mx-10">
      </div>

    </div>
  </body>
</template>
