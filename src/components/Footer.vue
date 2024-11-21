<template>
   <footer class="bg-gray-50 py-10 font-sans text-sm">
    <div class=" hf_paddingx container mx-auto  grid grid-cols-1 lg:grid-cols-3 gap-8 hf_paddingx">
        
        <!-- Columna 1: Logo y Descripción -->
        <div>
            <a href="index.html" class="block mb-4">
                <img src="../assets/img/logo.png" alt="Hostco Logo" class="w-50">
            </a>
            <p class="text-gray-600 mb-4 font-sans">
                We are Hostco, a web hosting company with 24/7 customer support. We provide best hosting solutions for your hosting needs. Our clients from personal to corporate. Our data centers are all over the world to ensure your website is always up. You can choose shared hosting, VPS hosting, or cloud hosting. You can also be a hosting reseller here. Happy hosting with us.
            </p>
            <h5 class="font-semibold text-gray-800 mb-2">We Accepted</h5>
            <div class="flex space-x-4">
                <img src="../assets/img/payments-logo/visa.png" alt="Visa" class="w-72px h-10">
                <img src="../assets/img/payments-logo/master-card.png" alt="MasterCard" class="w-72px h-10">
                <img src="../assets/img/payments-logo/jcb.png" alt="JCB" class="w- h-10">
                <img src="../assets/img/payments-logo/paypal.png" alt="PayPal" class="w-72px h-10">
            </div>
        </div>

        <!-- Columna 2: Enlaces de Hosting y Empresa -->
        <div>
            <div class="grid grid-cols-2 gap-4">
                <div>
                    <h5 class="font-semibold text-gray-800 mb-4">Hosting</h5>
                    <ul class="space-y-2 text-gray-600">
                        <li><a href="#" class="hover:text-gray-900">Web Hosting</a></li>
                        <li><a href="#" class="hover:text-gray-900">VPS Hosting</a></li>
                        <li><a href="#" class="hover:text-gray-900">Cloud Hosting</a></li>
                        <li><a href="#" class="hover:text-gray-900">WordPress Hosting</a></li>
                        <li><a href="#" class="hover:text-gray-900">Email Hosting</a></li>
                        <li><a href="#" class="hover:te10xt-gray-900">CMS Hosting</a></li>
                        <li><a href="#" class="hover:text-gray-900">Ecommerce Hosting</a></li>
                        <li><a href="#" class="hover:text-gray-900">Website Builder</a></li>
                    </ul>
                </div>
                <div>
                    <h5 class="font-semibold text-gray-800 mb-4">Company</h5>
                    <ul class="space-y-2 text-gray-600">
                        <li><a href="#" class="hover:text-gray-900">About</a></li>
                        <li><a href="#" class="hover:text-gray-900">Affiliates</a></li>
                        <li><a href="#" class="hover:text-gray-900">Blog</a></li>
                        <li><a href="#" class="hover:text-gray-900">Careers</a></li>
                        <li><a href="#" class="hover:text-gray-900">Community</a></li>
                        <li><a href="#" class="hover:text-gray-900">News</a></li>
                        <li><a href="#" class="hover:text-gray-900">Partners</a></li>
                        <li><a href="#" class="hover:text-gray-900">Press Releases</a></li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Columna 3: Newsletter y Redes Sociales -->
        <div>
            <h5 class="font-ElegantIcons text-gray-800 mb-4">Newsletter</h5>
            <p class="text-gray-600 mb-4">Signup for our newsletter to get the latest news in your inbox.</p>
            <form class="flex mb-4">
                <input type="email" placeholder="enter your email" class="w-full px-3 py-12px w-30px  border-gray-100 bg-gray-150  focus:outline-none focus:ring-2 focus:ring-blue-500" />
                <button type="submit" class=" font-bold px-10 py-3 bg-sky-400 text-white rounded-r-3xl hover:bg-sky-300 ">→</button>
            </form>
            <p class="text-gray-500 text-sm mb-4">Your email is safe with us. We don't spam.</p>
            <h5 class="font-semibold text-gray-800 mb-2">Follow Us on</h5>
            <div class="flex space-x-4 gap-3 py-4">
                <a href="#" class="text-sky-400 "><i class="fab fa-facebook fa-lg"></i></a>
                <a href="#" class="text-sky-400 "><i class="fab fa-twitter fa-lg"></i></a>
                <a href="#" class="text-sky-400"><i class="fab fa-linkedin fa-lg"></i></a>
                <a href="#" class="text-sky-400 "><i class="fab fa-pinterest fa-lg"></i></a>
                <a href="#" class="text-sky-400 "><i class="fas fa-rss fa-lg"></i></a>
            </div>
        </div>
    </div>

    <!-- Subfooter -->
    <div class="border-t border-gray-200 py-4 mt-auto flex justify-center content-end ">
        <div class="container mx-auto bg-gray-50 px-4 flex flex-col md:flex-row items-center justify-between text-gray-600 pb-4">
            <p class="text-sm">&copy; 2023 - Hostco by Designesia</p>
            <ul class="flex space-x-4 text-sm ">
                <li><a href="#" class="hover:text-gray-900">Terms & Conditions</a></li>
                <li><a href="#" class="hover:text-gray-900">Privacy Policy</a></li>
            </ul>
        </div>
    </div>
</footer>

</template>

<script setup>
const subscribe = () => {
   // Lógica para el formulario de suscripción
   console.log("Subscribed!");
};
</script>

<style scoped>
/* Si necesitas personalización adicional, puedes agregar estilos aquí */
</style>