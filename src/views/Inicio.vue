<script setup>
import Slide from '@/components/Inicio/Slide.vue';
import PanelFAQ from '../components/Inicio/PanelFAQ.vue';
import Banner from '../components/Inicio/Banner.vue';
import Testimonial from '@/components/Inicio/Testimonial.vue';
import Map from '@/components/Inicio/Map.vue';
import EasySteps from '@/components/Inicio/Easy Steps.vue';
import HostingPlan from '@/components/Inicio/HostingPlan.vue';
import ClientesSoportados from '@/components/Inicio/ClientesSoportados.vue';
import InformacionDestacada from '@/components/Inicio/InformacionDestacada.vue';
import VistaInicial from '@/components/Inicio/VistaInicial.vue';

</script>
<template>
   <div class="hf_paddingx">
      <VistaInicial/>
      <InformacionDestacada/>
      <ClientesSoportados />
      <HostingPlan />
      <EasySteps />
      <Map/>
      <Testimonial/>
      <Banner/>
      <PanelFAQ />
      <Slide/>

   </div>
</template>
<style scoped>

</style>