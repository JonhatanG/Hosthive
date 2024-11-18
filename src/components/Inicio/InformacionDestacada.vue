<template>
   <section class="bg-slate-50 py-12 font-sans pb-auto">
      <div class="container mx-auto grid grid-cols-1 md:grid-cols-2 items-center gap-8 px-6">
         <!-- Columna de la Imagen -->
         <div class="flex justify-center ">
            <img
               class="server anim-up-down lg:flex-1 hidden lg:block w-full max-w-md  "
               src="img/misc/server.png"
               alt="Server illustration"
            />
         </div>

         <!-- Columna del Texto -->
         <div class="flex flex-col justify-center text-left">
            <h2 class="text-4xl font-bold leading-tight mb-4">
               New functionality brings maximum 
               <span class="text-sky-400">power</span> to your website.
            </h2>
            <p class="text-gray-600 mb-6">
               Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam.
            </p>
            <!-- Lista de características -->
            <div class="grid grid-cols-2 gap-4 text-gray-800">
               <p class="flex items-center">
                  <span class="text-sky-400 text-xl mr-2">✔</span> Instant Activation
               </p>
               <p class="flex items-center">
                  <span class="text-sky-400 text-xl mr-2">✔</span> Reliable Hardware
               </p>
               <p class="flex items-center">
                  <span class="text-sky-400 text-xl mr-2">✔</span> 99.9% Uptime
               </p>
               <p class="flex items-center">
                  <span class="text-sky-400 text-xl mr-2">✔</span> 24 / 7 Support
               </p>
            </div>
            <!-- Botón -->
            <button class="mt-6 px-6 w-36 py-3 bg-blue-500 text-white font-semibold rounded-lg  transition focus:ring-2 hover:shadow-lg hover:shadow-sky-400">
               Learn More
            </button>
         </div>
      </div>
   </section>
</template>

<script>
export default {};
</script>

<style scoped>
@keyframes up-down {
  0%,
  100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-20px);
  }
}

.anim-up-down {
  animation: up-down 1s ease-in-out infinite;
}

button{

   @apply bg-sky-400  text-white font-semibold rounded-full 
}
</style>
