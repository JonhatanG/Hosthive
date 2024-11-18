<template>
   <section class="container font-sans">

      <div class="flex flex-col py-7 items-center text-center space-y-2 ">
         <span class="bg-sky-200 px-4 py-1  rounded-full text-xs  tracking-wide text-sky-400">TESTIMONIALS</span>
         <div class="trust text-center py-7 text-4xl font-bold flex-wrap">Trusted by over 5,000
            <br>happy customers<span class="world text-sky-300"> worldwide</span> </div>
         <span class="text-18px  text-lg text-center text-gray-500 font-semibold  ">Sit labore et officia eiusmod tempor officia eiusmod dolor
            exercitation
            <br>nulla dolore ut id velit et ut anim.</span>
      </div>
   </section>
   <Splide :options="splideOptions" class="testimonial-carousel font-sans">
      <SplideSlide v-for="(testimonialSet, index) in splitTestimonials" :key="index" class="p-16">
         <div class="flex justify-around gap-6">
            <div v-for="(testimonial, i) in testimonialSet" :key="i"
               class="testimonial-card relative p-6 bg-white rounded-lg shadow-md text-start max-w-sm">

               <!-- Contenedor del ícono de la cita -->
               <div
                  class="quote-icon-container absolute top-0  left-0  bg-sky-400 text-white w-16 h-16 rounded-tr-lg flex items-center justify-center">
                  <span class="text-3xl">❝</span>
               </div>

               <!-- Contenido del testimonial -->
               <h3 class="text-lg font-bold mt-12 mb-2">{{ testimonial.title }}</h3>
               <p class="text-gray-700 mb-4">{{ testimonial.message }}</p>
               <div class="author flex items-center justify-center">
                  <img :src="testimonial.image" class="h-12 w-12 rounded-full mr-3"
                     alt="Foto de {{ testimonial.author }}" />
                  <div class="text-left">
                     <p class="font-semibold">{{ testimonial.author }}</p>
                     <p class="text-sm text-gray-500">{{ testimonial.company }}</p>
                  </div>
               </div>
            </div>
         </div>
      </SplideSlide>
   </Splide>
</template>

<script setup>
import { ref } from 'vue';
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import '@splidejs/splide/dist/css/splide.min.css';

// Definir los testimonios como una referencia, usando imágenes públicas de prueba
const testimonials = ref([
   {
      title: 'Excellent Hosting',
      message: 'Great support, like I have never seen before. Thanks to the support team, they are very helpful. This company provides customers great solutions that make them the best.',
      author: 'Michael',
      company: 'Apple',
      image: require('@/assets/img/team/1.jpg'),
   },
   {
      title: 'Great Experience',
      message: 'I am very pleased with the services provided. The team is professional and always ready to assist with any issues I have.',
      author: 'Sarah',
      company: 'Google',
      image: require('@/assets/img/team/4.jpg')
   },
   {
      title: 'Reliable Service',
      message: 'Hosting is incredibly reliable and the uptime is top-notch. The team makes me feel secure about my website.',
      author: 'John',
      company: 'Microsoft',
      image: require('@/assets/img/team/team_pic_5.jpg')
   },
   {
      title: 'Fantastic Support',
      message: 'The support team is the best I have encountered, they really care about helping their customers.',
      author: 'Emma',
      company: 'Amazon',
      image: require('@/assets/img/team/team_pic_2.jpg')
   },
   {
      title: 'Highly Recommend',
      message: 'I would highly recommend this hosting service to anyone looking for reliable and professional hosting.',
      author: 'Robert',
      company: 'Tesla',
      image: require('@/assets/img/team/team_pic_1.jpg'),
   },
   {
      title: 'Exceptional Value',
      message: 'The value for money is incredible, and the support team makes it even better.',
      author: 'Alice',
      company: 'Meta',
      image: require('@/assets/img/team/team_pic_8.jpg')
   }
]);

// Agrupar los testimonios en grupos de 3 para tener 2 slides
const splitTestimonials = ref([
   testimonials.value.slice(0, 3),
   testimonials.value.slice(3, 6)
]);

// Opciones para Splide
const splideOptions = ref({
   type: 'loop',       // Loop continuo para que el carrusel sea infinito
   perPage: 1,         // Mostrar 1 "slide" a la vez (cada "slide" contiene 3 contenedores)
   autoplay: true,     // Autoplay habilitado
   interval: 3000,     // Intervalo entre cada slide (en ms)
   speed: 800,         // Velocidad de la transición (en ms)
   arrows: false,      // Ocultar los botones de navegación
   pagination: true,   // Mostrar indicadores de paginación
});
</script>

<style scoped>
.testimonial-card {
   background: #F0F9FE;
   box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
   padding-top: 4rem;
   /* Aumentar el espacio para el ícono de la cita */
   position: relative;
}

.quote-icon-container {
   width: 4rem;
   height: 4rem;
   display: flex;
   align-items: center;
   justify-content: center;
   border-radius: 0 0 15px 0;
}

/* Estilos para los botones de paginación */
.splide__pagination {
   position: relative;
   bottom: -30px;
   /* Aumentar la separación de la paginación hacia abajo */
   margin-top: 20px !important;
}

.splide__pagination__page {
   background-color: #60a5fa !important;
   /* Color sky-400 */
   width: 16px !important;
   height: 30px !important;
   margin: 0 12px !important;
   /* Aumenta el espacio entre cada botón de paginación */
   border-radius: 50%;
   /* Asegura que los botones sean redondos */
}

.splide__pagination__page.is-active {
   background-color: #3b82f6 !important;
   /* Color sky-500 para el botón activo */
}
</style>
