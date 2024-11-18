<template>
  <section class="container mx-auto font-sans bg-slate-50 text-gray-700 py-8 px-4">
    <div class="text-center mb-8 flex flex-col items-center">
      <p class="bg-sky-200 px-4 py-1 rounded-full text-xs tracking-wide text-sky-400">Easy Steps</p>
      <h2 class="text-3xl font-bold text-gray-800 py-6">How It Works</h2>
      <p class="text-gray-500">Sit labore et officia eiusmod tempor officia eiusmod dolor exercitation <br> nulla dolore ut
        id velit et ut anim.</p>
    </div>

    <!-- Steps Container with Border Line -->
    <div class="relative">
      <!-- Horizontal Line -->
      <div class="absolute inset-x-0 top-1/2 border-t border-sky-300 z-0"></div>

      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 text-center relative z-10">
        <div class="flex flex-col items-center">
          <div
            class="bg-sky-300 text-white rounded-lg h-12 w-12 flex items-center justify-center text-lg font-bold hover:bg-sky-400 relative z-10">
            1</div>
          <h3 class="text-xl font-semibold mt-4">Select Plan</h3>
          <p class="mt-2 text-gray-500">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
            incididunt ut labore.</p>
        </div>
        <div class="flex flex-col items-center">
          <div
            class="bg-sky-300 text-white rounded-lg h-12 w-12 flex items-center justify-center text-lg font-bold hover:bg-sky-400 relative z-10">
            2</div>
          <h3 class="text-xl font-semibold mt-4">Choose Domain</h3>
          <p class="mt-2 text-gray-500">Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
            fugiat nulla pariatur.</p>
        </div>
        <div class="flex flex-col items-center">
          <div
            class="bg-sky-300 text-white rounded-lg h-12 w-12 flex items-center justify-center text-lg font-bold hover:bg-sky-400 relative z-10">
            3</div>
          <h3 class="text-xl font-semibold mt-4">Login/Register</h3>
          <p class="mt-2 text-gray-500">Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo.</p>
        </div>
        <div class="flex flex-col items-center">
          <div
            class="bg-sky-300 text-white rounded-lg h-12 w-12 flex items-center justify-center text-lg font-bold hover:bg-sky-400 relative z-10">
            4</div>
          <h3 class="text-xl font-semibold mt-4">Make Payment</h3>
          <p class="mt-2 text-gray-500">Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
            aliquip ex ea commodo.</p>
        </div>
      </div>
    </div>
  </section>
</template>
