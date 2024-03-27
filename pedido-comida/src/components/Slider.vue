<template>
  <div class="my-slider-wrapper">
    <swiper
      :pagination="{
        dynamicBullets: true,
      }"
      :modules="modules"
      class="mySwiper"
    >
    <swiper-slide class="text-center">
      <div class="flex mt-10 ml-20">
        <div class="w-1/2 flex flex-col justify-center items-center custom-rotation mb-40">
          <span class="text-2xl font-bold text-amber-400 ml-20 ">Ricas</span> 
          <div class="flex flex-col items-start"> 
              <h1 class="concert-one-regular text-6xl flex">Hamburguesas <div class="text-black ml-5 mx-auto container bg-amber-400 w-20 h-20">$$ <br></div></h1>
              <p class="concert-one-regular text-left truncate">¡Saborea nuestras hamburguesas en RocoDog! Jugosas, sabrosas y siempre frescas. <br> Ven y descubre el auténtico sabor de la perfección. ¡No te lo pierdas!</p>
          </div>
      </div>    
        <div class="w-1/2 ">
          <img class="w-4/5 h-auto" src="../assets/img/hamburguesa-slider.png" alt="">
          
      </div>  
      </div>
  </swiper-slide>
  
      <swiper-slide class="text-center">
        <div class="flex ml-30">
          <div class="w-1/2 flex flex-col justify-center items-center custom-rotation mb-40">
            <span class="text-2xl font-bold text-amber-400 ml-20 ">Ricos</span> 
            <div class="flex flex-col items-start"> 
                <h1 class="concert-one-regular text-6xl flex">Completos <div class="text-black ml-5 mx-auto container bg-amber-400 w-20 h-20">$$ <br></div></h1>
                <p class="concert-one-regular text-left truncate">¡Saborea nuestras hamburguesas en RocoDog! Jugosas, sabrosas y siempre frescas. <br> Ven y descubre el auténtico sabor de la perfección. ¡No te lo pierdas!</p>
            </div>
        </div>    
          <div class="w-1/2 ">
            <img class="w-4/5 h-auto mb-40" src="../assets/img/slider-2.png" alt="">
            
        </div>  
        </div>
      </swiper-slide>
      <swiper-slide class="text-center">
        <div class="flex mt-20 ml-20">
          <div class="w-1/2 flex flex-col justify-center items-center custom-rotation ">
            <span class="text-2xl font-bold text-amber-400 ml-20 ">Ricos</span> 
            <div class="flex flex-col items-start"> 
                <h1 class="concert-one-regular text-6xl flex">Churrascos <div class="text-black ml-5 mx-auto container bg-amber-400 w-20 h-20">$$ <br></div></h1>
                <p class="concert-one-regular text-left truncate">¡Saborea nuestras hamburguesas en RocoDog! Jugosas, sabrosas y siempre frescas. <br> Ven y descubre el auténtico sabor de la perfección. ¡No te lo pierdas!</p>
            </div>
        </div>    
          <div class="w-1/2 ">
            <img class="w-auto h-auto" src="../assets/img/slider-3.png" alt="">
            
        </div>  
        </div>
      </swiper-slide>
      <swiper-slide class="text-center">
        <div class="flex mt-20 ml-20">
          <div class="w-1/2 flex flex-col justify-center items-center custom-rotation ">
            <span class="text-2xl font-bold text-amber-400 ml-20 ">Ricas</span> 
            <div class="flex flex-col items-start"> 
                <h1 class="concert-one-regular text-6xl flex">Chorrillanas <div class="text-black ml-5 mx-auto container bg-amber-400 w-20 h-20">$$ <br></div></h1>
                <p class="concert-one-regular text-left truncate">¡Saborea nuestras hamburguesas en RocoDog! Jugosas, sabrosas y siempre frescas. <br> Ven y descubre el auténtico sabor de la perfección. ¡No te lo pierdas!</p>
            </div>
        </div>    
          <div class="w-1/2 ">
            <img class="w-auto h-auto" src="../assets/img/slider-4.png" alt="">
            
        </div>  
        </div>
      </swiper-slide>
      
    </swiper>

    <div class="swiper-pagination"></div>
  </div>
  </template>
  
  <script>
  import { Swiper, SwiperSlide } from 'swiper/vue';
  import 'swiper/css';
  import { Pagination } from 'swiper/modules';
  
  export default {
    name: "MySlider",
   
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {
        modules: [Pagination],
      };
    },
  };
  </script>
  
  <style scoped>
  .my-slider-wrapper {
    height: 100%;
    overflow: hidden;
  }
  </style>
  