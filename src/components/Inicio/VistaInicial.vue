<template>
  <section class="py-0 bg-gray-50 font-sans ">
    <div class="container mx-auto   ">
      <!-- Contenedor de dos columnas -->
      <div class="grid grid-cols-1 sm:grid-cols-2 gap-8 items-center ">
        <!-- Texto y formulario -->
        <div>
          <h1 class="text-5xl font-bold py-8  ">
            Premium hosting for <br />
            everyone, <span class="text-sky-400">small</span> or <span class="text-sky-400">large</span>
          </h1>
          <p class="text-lg text-gray-600 mb-6">
            High performance secured hosting for your website. Don't lose anymore <br />
            clients for the slowest speed of your hosting service.
          </p>
          <!-- Formulario -->
          <form class="flex items-center mb-4">
            <input
              type="email"
              placeholder="enter domain name"
              class="flex-1 px-4 py-3 border  border-gray-300 bg-gray-50 rounded-l-full focus:outline-none focus:ring- focus:ring-blue-500"
            />
            <button
              type="submit"
              class="px-6 py-4 bg-sky-400 text-white font-bold rounded-r-3xl hover:bg-sky-500 transition-colors"
            >
              →
            </button>
          </form>
          <h4 class="text-xs text-gray-500 mb-4">
            *Reserve your domain today before someone take it.
          </h4>
          <!-- Lista de dominios con precios -->
          <div class="flex justify-start gap-12 2 flex-wrap">
            <div>
              <h4 class="text-sky-500 text-lg font-bold">.com</h4>
              <p class="text-gray-600 text-sm font-normal">$4.99/year</p>
            </div>
            <div>
              <h4 class="text-sky-500 text-lg font-bold">.net</h4>
              <p class="text-gray-600 text-sm font-normal">$3.99/year</p>
            </div>
            <div>
              <h4 class="text-sky-500 text-lg font-bold">.co</h4>
              <p class="text-gray-600 text-sm font-normal">$2.99/year</p>
            </div>
            <div>
              <h4 class="text-sky-500 text-lg font-bold">.info</h4>
              <p class="text-gray-600 text-sm font-normal">$3.90/year</p>
            </div>
            <div>
              <h4 class="text-sky-500 text-lg font-bold">.biz</h4>
              <p class="text-gray-600 text-sm font-normal">$5.99/year</p>
            </div>
          </div>
        </div>
        <!-- Imagen -->
        <div class="flex justify-center">
          <img
            class="server2 anim-up-down lg:flex-1 hidden lg:block w-full max-w-2xl"
            src="img/misc/server-2.png"
            alt="Server2 "
          />
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
@keyframes up-down {
  0%,
  100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-4px);
  }
}

.anim-up-down {
  animation: up-down 1s ease-in-out infinite;
}

button{

   @apply bg-sky-400  text-white font-semibold rounded-l-none 
}
</style>

