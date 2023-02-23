<template>
    <header class="bg-[url('./assets/fondo.png')]">
    <img
      alt="Rick and Morty logo"
      class="logo pl-8 mx-12 my-5"
      src="@/assets/Rick_and_Morty.svg"
      width="350"
      height="250"
    />

    <div class="wrapper p-10 text-right text-3xl text-green-500 font-black font-mono shadow-black">
      <nav>
        <RouterLink to="/" class="mr-5 ml-14 p-10">Inicio</RouterLink>
        <RouterLink to="/personajes" class="mr-5 p-10">Personajes</RouterLink>
        <RouterLink to="/about" class="mr-5 p-9">Acerca de</RouterLink>
      </nav>
    </div>
  </header>
</template>