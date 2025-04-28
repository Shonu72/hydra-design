<template>
    <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8 mt-2 justify-between">

        <!-- Hero Section -->
        <div class="grid grid-cols-2">
            <div class=" mt-20 ml-10">
                <h1 class="text-5xl text-white font-bold"><span class="text-purple-500">Dive</span> into The Depths</h1>
                <h1 class="text-5xl mt-2 text-white font-bold">of <span class="text-purple-500 ">Virtual Reality</span>
                </h1>
                <p class="mt-5 text-white">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente alias
                    accusantium animi officiis. Ipsa adipisci quia minima laudantium quidem quibusdam. Quidem corporis
                    quasi eveniet beatae nulla earum tempora molestiae est.</p>
                <div class="flex space-x-2 pt-2 mt-10">
                    <button type="button"
                        class="relative rounded-3xl text-sm font-medium text-purple focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-gray-800  hover:from-blue-600 hover:to-purple-700 transition-all duration-200 px-10 py-2 bg-gradient-to-r from-purple-400 to-gray-500 mr-7">
                        BUILD YOUR WORLD
                    </button>
                    <button type="button" class="relative rounded-3xl p-0 bg-transparent">
                        <img src="~assets/right-arrow.png" alt="" class="h-6 w-auto rounded-3xl" />
                    </button>
                </div>
            </div>
            <img src="~assets/hero2.png" alt="" class="img ml-20" height="450px" width="450px" />
        </div>

        <div class="w-full text-white rounded-full mb-4 radial-bg">
            <div class="max-w-6xl mx-auto px-4 ">
                <!-- Grid Container -->
              <div class="grid grid-cols-1 md:grid-cols-3 gap-8 justify-items-center">
  <!-- Visit Section -->
  <div class="flex items-center space-x-4 p-4 w-full relative">
    <!-- Vertical divider positioned between this and next item -->
    <div class="hidden md:block absolute -right-4 top-1/2 transform -translate-y-1/2 w-px h-16 bg-gray-700"></div>
    
    <!-- Location Icon -->
    <div class="flex-shrink-0 bg-purple-600 p-3 rounded-full">
      <svg class="h-5 w-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/>
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/>
      </svg>
    </div>
    <div>
      <h3 class="font-bold">Pay Us a Visit</h3>
      <p class="text-gray-300 text-sm">Union St. Seattle, WA 98101</p>
    </div>
  </div>
  
  <!-- Call Section -->
  <div class="flex items-center space-x-4 p-4 w-full relative">
    <!-- Vertical divider positioned between this and next item -->
    <div class="hidden md:block absolute -right-4 top-1/2 transform -translate-y-1/2 w-px h-16 bg-gray-700"></div>
    
    <!-- Phone Icon -->
    <div class="flex-shrink-0 bg-purple-600 p-3 rounded-full">
      <svg class="h-5 w-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"/>
      </svg>
    </div>
    <div>
      <h3 class="font-bold">Give Us a Call</h3>
      <p class="text-gray-300 text-sm">(NO) 111-1010</p>
    </div>
  </div>
  
  <!-- Message Section -->
  <div class="flex items-center space-x-4 p-4 w-full">
    <!-- Email Icon -->
    <div class="flex-shrink-0 bg-purple-600 p-3 rounded-full">
      <svg class="h-5 w-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/>
      </svg>
    </div>
    <div>
      <h3 class="font-bold">Send Us a Message</h3>
      <p class="text-gray-300 text-sm">Contact@HydraVTech.com</p>
    </div>
  </div>
</div>
            </div>
        </div>



    </div>


</template>

<script setup>

</script>

<style scoped>
.radial-bg {
    background: radial-gradient(circle at center, #3A3456 0%, #211E2E 100%);
}
</style>