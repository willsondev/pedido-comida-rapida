<template>
  
  <div class="my-slider-wrapper">
    <swiper
    :pagination="{
      clickable: true,
    }"
    :navigation="{
      nextEl: '.swiper-button-next',
      prevEl: '.swiper-button-prev',
    }"
    :modules="modules"
    class="mySwiper"
    :autoplay="{
      delay: 5000, // Cambiar cada 5 segundos (ajusta este valor según tus necesidades)
      disableOnInteraction: false, // Desactiva la pausa automática al interactuar con el slider
    }"
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
        <div class="flex ml-40 ">
          <div class="w-1/2 flex flex-col justify-center items-center custom-rotation mb-60">
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
        <div class="flex  ml-40">
          <div class="w-1/2 flex flex-col justify-center items-center custom-rotation mb-60">
            <span class="text-2xl font-bold text-amber-400 ml-20 ">Ricos</span> 
            <div class="flex flex-col items-start"> 
                <h1 class="concert-one-regular text-6xl flex">Churrascos <div class="text-black ml-5 mx-auto container bg-amber-400 w-20 h-20">$$ <br></div></h1>
                <p class="concert-one-regular text-left truncate">¡Saborea nuestras hamburguesas en RocoDog! Jugosas, sabrosas y siempre frescas. <br> Ven y descubre el auténtico sabor de la perfección. ¡No te lo pierdas!</p>
            </div>
        </div>    
          <div class="w-1/2 mb-40">
            <img class="w-4/5 h-auto " src="../assets/img/slider-3.png" alt="">
            
        </div>  
        </div>
      </swiper-slide>
      <swiper-slide class="text-center">
        <div class="flex  ml-40">
          <div class="w-1/2 flex flex-col justify-center items-center custom-rotation mb-20">
            <span class="text-2xl font-bold text-amber-400 ml-20 ">Ricas</span> 
            <div class="flex flex-col items-start"> 
                <h1 class="concert-one-regular text-6xl flex">Chorrillanas <div class="text-black ml-5 mx-auto container bg-amber-400 w-20 h-20">$$ <br></div></h1>
                <p class="concert-one-regular text-left truncate">¡Saborea nuestras hamburguesas en RocoDog! Jugosas, sabrosas y siempre frescas. <br> Ven y descubre el auténtico sabor de la perfección. ¡No te lo pierdas!</p>
            </div>
        </div>    
          <div class="w-1/2 ">
            <img class="w-4/5 h-auto" src="../assets/img/slider-4.png" alt="">
            
        </div>  
        </div>
      </swiper-slide>
      
    
    </swiper>

   
    <div class="swiper-button-next  "></div>
      <div class="swiper-button-prev"></div>
  </div>
  </template>
  
  <script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import { Pagination, Navigation, Autoplay } from 'swiper/modules';
import 'swiper/css/pagination';

export default {
  name: "MySlider",
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Pagination, Navigation, Autoplay],
    };
  },
};
</script>

<style scoped>
.my-slider-wrapper {
  height: 100%;
  overflow: hidden;
}

.swiper-button-next{
  position: absolute;
  top: 80%;
  left: 10%;
  transform: translateY(50%);
  width: 40px;
  height: 40px;
  cursor: pointer;
  z-index: 9999; /* Ajusta el z-index según sea necesario */
}
.swiper-button-prev {
  position: absolute;
  top: 86%;
  left: 5%;
  transform: translateY(-50%);
  width: 40px;
  height: 40px;
  cursor: pointer;
  z-index: 9999; /* Ajusta el z-index según sea necesario */
}

.swiper-button-next::after {
  content: '>';
  position: absolute;
  top: 50%;
  left: 50%;
  font-size: 75px; /* Ajusta el tamaño del texto según sea necesario */
  transform: translate(-50%, -50%);
}
.swiper-button-prev::after {
  content: '<';
  position: absolute;
  top: 50%;
  left: 50%;
  font-size: 70px; /* Ajusta el tamaño del texto según sea necesario */
  transform: translate(-50%, -50%);
}

.swiper-button-prev::after {
  transform: translate(-50%, -50%) rotate(0deg);
}

.swiper-button-next::after {
  transform: translate(-50%, -50%) rotate(0deg);
}
</style>
  