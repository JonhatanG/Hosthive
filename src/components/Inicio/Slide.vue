<template>
  <Splide :options="splideOptions" class="logo-carousel">
    <SplideSlide v-for="(image, index) in images" :key="index">
      <img :src="image" :alt="`Logo ${index + 1}`" class="h-24 w-22 object-contain hover:scale-105 transition-transform duration-300" />
    </SplideSlide>
  </Splide>
</template>

<script setup>
import { ref } from 'vue';
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import '@splidejs/splide/dist/css/splide.min.css';

// Definir las imágenes como una referencia para usarlas en el template
const images = ref([
  require('@/assets/img/logo/1.png'),
  require('@/assets/img/logo/2.png'),
  require('@/assets/img/logo/3.png'),
  require('@/assets/img/logo/4.png'),
  require('@/assets/img/logo/5.png'),
  require('@/assets/img/logo/6.png'),
  require('@/assets/img/logo/7.png'),
  require('@/assets/img/logo/8.png'),
]);

// Opciones para Splide
const splideOptions = ref({
  type: 'loop',       // Loop continuo para que el carrusel sea infinito
  perPage: 4,         // Mostrar 4 imágenes al mismo tiempo (ajustar según el diseño)
  autoplay: true,     // Autoplay habilitado
  interval: 3000,     // Intervalo entre cada slide (en ms)
  speed: 1500,         // Velocidad de la transición (en ms)
  arrows: false,      // Ocultar los botones de navegación
  pagination: false,  // Ocultar los indicadores de paginación
  pauseOnHover: false // No pausar al hacer hover
});
</script>

<style scoped>
.logo-carousel img {
  transition: transform 0.5s ease-in-out;
  width: 100%;
  height: auto;
  object-fit: contain;
}
</style>
