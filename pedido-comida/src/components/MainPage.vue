<template>
  <div class="main-page bg-custom-black">
    <header class="text-white w-3/4 mx-auto flex justify-between items-center h-30">
      <nav class="flex gap-48 text-lg items-center">
        <span class="text-amber-400">Inicio</span>
        <span>Sobre mí</span>
        <span class="w-20"><img src="../assets/img/logo.png" alt=""></span>
        <span>Proyectos</span>
        <span class="flex items-center">Contacto <img class="w-10" src="../assets/img/logo.png" alt=""></span>
      </nav>
    </header>
  
    <section class="text-white seccion-uno flex justify-center items-center ">
      <Slider />
    </section>
  </div>
</template>

<script>
import Slider from '../components/Slider.vue';

export default {
  name: 'MainPage',
  components: {
    Slider
  }
}
</script>

<style scoped>
.main-page {
  height: 100vh; /* Establece la altura al 100% del tamaño de la ventana */
  overflow: hidden; /* Evita el desplazamiento vertical */
}

.seccion-uno {
  height: calc(100vh - 30px); /* Calcula el tamaño de la sección descontando la altura del encabezado */
}
</style>
