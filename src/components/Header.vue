  <template>
    <header class= "bg-white shadow-md font-sans w-full ">
      <div id="topbar " class="bg-sky-100 py-2 text-gray-600 ">
        <div class="  container  mx-auto flex justify-between items-center hf_paddingx ">
          <!-- Left Side -->
          <div class=" hidden sm:block ">
            <a href="#" class="text-sm font-semibold hover:text-gray-800">Get Free Shared Hosting!</a>
          </div>

          <!-- Right Side -->
          <div class="flex space-x-4 ">
            <a href="#" class="flex items-center text-sm font-semibold hover:text-gray-800">
              <i class="fa fa-phone mr-1 text-sky-400"></i> +208 333 9296
            </a>
            <a href="#" class="flex items-center text-sm font-semibold hover:text-gray-800">
              <i class="fa fa-envelope mr-1  text-sky-400"></i> support@hostco.com
            </a>
          </div>
        </div>
      </div>

      <div class="container mx-auto ">
        <div class=" flex justify-evenly items-end py-4 hf_paddingx">
          <!-- Logo -->
          <div id="logo">
            <a href="index.html">
              <img class="hidden md:block w-50" src="../assets/img/logo.png" alt="Logo principal">
              <img class="block md:hidden w-20" src="../assets/img/logo-mobile.png" alt="Logo móvil">
            </a>
          </div>

          <!-- Menu -->
          <nav class="hidden lg:flex space-x-8 items-center">
            <a href="index.html" class="text-gray-700 font-semibold hover:text-cyan-300">Home</a>
            <div class="relative group">
              <a href="hosting-shared.html" class="text-gray-700 font-semibold hover:text-sky-400">Hosting</a>
              <div class="absolute hidden group-hover:block bg-white shadow-lg top-full mt-2 p-4 w-80">
                <h4 class="font-semibold mb-2">Hosting Made Easy</h4>
                <p class="text-sm text-gray-600 mb-4">High performance secured hosting for your website.</p>
                <a href="hosting-shared.html" class="flex items-center mb-2 text-blue-600 hover:underline">
                  <img src="../assets/img/svg/server-svgrepo-com.svg" class="w-5 h-5 mr-2" alt="Icono servidor"> Shared Hosting
                </a>
                <a href="hosting-cloud.html" class="flex items-center text-blue-600 hover:underline">
                  <img src="../assets/img/svg/cloud-svgrepo-com.svg" class="w-5 h-5 mr-2" alt="Icono nube"> Cloud Hosting
                </a>
              </div>
            </div>
            <a href="domain.html" class="text-gray-700 font-semibold hover:text-sky-400">Domain</a>
            <a href="website-builder.html" class="text-gray-700 font-semibold hover:text-sky-400">Websites</a>
            <a href="help-center.html" class="text-gray-700 font-semibold hover:text-sky-400">Help</a>
            <a href="#" class="text-gray-700 font-semibold hover:text-sky-400">Pages</a>
            <a href="#" class="text-gray-700 font-semibold hover:text-sky-400">More</a>
          </nav>

          
          <div class="flex items-center  space-x-4 ">
            <a href="login.html" class="btn-main px-7 py-3 focus:ring-2 bg-blue-600 text-white rounded-r-full hover:shadow-lg hover:shadow-sky-400">Free Trial</a>
            <span id="menu-btn" class=" boton lg:hidden text-gray-700 cursor-pointer flex  ">☰</span>
          </div>
        </div>
      </div>
    </header>
  </template>

  <style scoped>
  .btn-main {
    @apply bg-sky-400 text-white font-semibold rounded-full ;
  }

  .boton{

    
  }
  </style>

  <script setup>

  </script>
