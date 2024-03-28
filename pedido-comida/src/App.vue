<template>
  <div id="app">
    <MainPage />
    <MenuPageVue/>
    
   
  </div>
</template>

<script>
import MainPage from './components/MainPage.vue';
import MenuPageVue from './components/MenuPage.vue';



export default {
  name: 'App',
  components: {
    MainPage,
    MenuPageVue
    
    
  }
}
</script>

<style>
/* Estilos globales de la aplicación */
</style>
