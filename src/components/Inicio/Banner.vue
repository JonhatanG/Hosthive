<template>
   <section id="section-banner" class="no-bottom no-top h-100 bg-sky-100 text-lg font-sans p8">
      <div class="container mx-auto">
         <div class="flex flex-wrap items-center ">
            <div class="lg:flex-1 hidden lg:block text-center">
               <img class=" w-full mt-16" src="/img/misc/1.png" alt="Banner Image">
            </div>

            <div class="lg:flex-1 md:w-1/2 p-6">
               <h2 class="text-4xl font-bold"><span class="text-gradient">30 days</span> money back guarantee</h2>
            </div>

            <div class="lg:flex-1 md:w-1/2 p-10">
               <div class="space-y-4">
                  <p class="text-l mb-12 ">If you are not satisfied, we will refund your payment. No hassle, no risk. You can
                     cancel the plan at any time.</p>
                  <a class="btn-main bg-sky-400 text-white py-2 px-4 font-semibold  rounded-full" href="#">Get Started</a>
                  <p class="text-sm   mb-12 ">*Cancellation must be within a maximum of 30 days</p>
               </div>
            </div>
         </div>
      </div>
   </section>
</template>

<script setup>
// No es necesario agregar lógica específica en el script para esta estructura
</script>

<style scoped>
.text-gradient {
   background: linear-gradient(to right, #58cbf1, #b1e2ed);
   -webkit-background-clip: text;
   -webkit-text-fill-color: transparent;
}
</style>