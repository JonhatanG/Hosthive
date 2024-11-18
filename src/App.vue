<script setup>
import Footer from './components/Footer.vue';

import Header from './components/Header.vue';


</script>

<template>
  <div >
    <Header />
    <router-view></router-view>
    <Footer />
  </div>

  <!-- <router-link to="/">Home</router-link> | -->

</template>


<style>
.hf_paddingx {
  @apply px-24;
}

.color_primary{
  color: rgb(56 189 248)
}

</style>
