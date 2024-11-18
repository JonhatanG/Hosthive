<template>
  <section id="section-faq" class="py-12 bg-gray-50 font-sans">
    <div class="container mx-auto">
      <!-- Título -->
      <div class="text-center mb-10 flex flex-col items-center">
        <p class="bg-sky-200 px-4 py- rounded-full text-xs tracking-wide text-sky-400">DO YOU HAVE</p>
        <h2 class="text-4xl font-semibold text-black pt-20 pb-4">Any Questions?</h2>
      </div>

      <!-- Grid de preguntas frecuentes -->
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8 ">
        <!-- Pregunta 1 -->
        <div class="space-y-4">
          <button @click="toggleContent(1)" class=" font-semibold text-gray-700  rounded ">
            How do I get started with web hosting?
          </button>
          <transition name="slide-fade">
            <div v-if="activeSection === 1" class=" transition-height duration-1000 overflow-hidden">

              <p class="text-gray-400 mt-2 ">AAt vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis
                praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati
                cupiditate non provident, similique sunt in culpa qui officia deserunt mollitia animi, id est laborum et
                dolorum fuga. Et harum quidem rerum facilis est et expedita distinctio.</p>
            </div>
          </transition>
        </div>

        <!-- Pregunta 2 -->
        <div class="space-y-4">
          <button @click="toggleContent(2)" class=" font-semibold text-gray-700  rounded ">
            What is the difference for each plan?
          </button>
          <transition name="slide-fade">
            <div v-if="activeSection === 2" class="  transition-height duration-1000 overflow-hidden">

              <p class="text-gray-400 mt-2">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis
                praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati
                cupiditate non provident, similique sunt in culpa qui officia deserunt mollitia animi, id est laborum et
                dolorum fuga. Et harum quidem rerum facilis est et expedita distinctio.</p>
            </div>
          </transition>
        </div>

        <!-- Pregunta 3 -->
        <div class="space-y-4">
          <button @click="toggleContent(3)" class="font-semibold text-gray-700  rounded">
            What kind of web hosting do I need?
          </button>
          <transition name="slide-fade">
            <div v-if="activeSection === 3" class=" transition-height duration-1000 overflow-hidden">
              <p class="text-gray-400 mt-2">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis
                praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati
                cupiditate non provident, similique sunt in culpa qui officia deserunt mollitia animi, id est laborum et
                dolorum fuga. Et harum quidem rerum facilis est et expedita distinctio.
              </p>
            </div>
          </transition>
        </div>

        <!-- Pregunta 4 -->
        <div class="space-y-4">
          <button @click="toggleContent(4)" class="font-semibold text-gray-700 rounded">
            Why do I need a domain name?
          </button>
          <transition name="slide-fade">
            <div v-if="activeSection === 4" class=" transition-height duration-1000 overflow-hidden">

              <p class="text-gray-400 mt-2">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis
                praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati
                cupiditate non provident, similique sunt in culpa qui officia deserunt mollitia animi, id est laborum et
                dolorum fuga. Et harum quidem rerum facilis est et expedita distinctio.
              </p>
            </div>
          </transition>
        </div>

        <!-- Pregunta 5 -->
        <div class="space-y-4">
          <button @click="toggleContent(5)" class="font-semibold text-gray-700  rounded">
            Is my website protected from hackers?
          </button>
          <transition name="slide-fade">
            <div v-if="activeSection === 5" class=" transition-height duration-1000 overflow-hidden">

              <p class="text-gray-400 mt-2">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis
                praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati
                cupiditate non provident, similique sunt in culpa qui officia deserunt mollitia animi, id est laborum et
                dolorum fuga. Et harum quidem rerum facilis est et expedita distinctio.
              </p>
            </div>
          </transition>
        </div>

        <!-- Pregunta 6 -->
        <div class="space-y-4">
          <button @click="toggleContent(6)" class="font-semibold text-gray-700 rounded">
            How do I backup my website?
          </button>
          <transition name="slide-fade">
            <div v-if="activeSection === 6" class="transition-height duration-1000 overflow-hidden">
              <h3 class="font-semibold text-gray-700">How do I backup my website?</h3>
              <p class="text-gray-400 mt-2">At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis
                praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati
                cupiditate non provident, similique sunt in culpa qui officia deserunt mollitia animi, id est laborum et
                dolorum fuga. Et harum quidem rerum facilis est et expedita distinctio.
              </p>
            </div>
          </transition>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';

const activeSection = ref(null);

const toggleContent = (section) => {
  activeSection.value = activeSection.value === section ? null : section;
};
</script>

<style>
.transition-height {
  transition: height 1s ease;
}

.slide-fade-enter-active,
.slide-fade-leave-active {
  transition: opacity 1s ease;

}

.slide-fade-enter-from,
.slide-fade-leave-to {
  opacity: 0;
  height: 100;

}
</style>
