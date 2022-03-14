<template>
  
    <div class="max-w-7xl mx-auto px-4 sm:px-6">
      <div
        class="
          flex
          justify-between
          items-center
          border-b-2 border-gray-100
          py-6
          md:justify-start md:space-x-10
        "
      >
        <div class="flex justify-start  lg:flex-1">
          <a href="#">
            <span class="sr-only">Workflow</span>
            <h1>Muhabbet</h1>
          </a>
        </div>
        <div class="md:flex items-center justify-end ">
          <a
            :href="route('chat')"
            class="
              ml-8
              whitespace-nowrap
              inline-flex
              items-center
              justify-center
              px-4
              py-2
              border border-transparent
              rounded-md
              shadow-sm
              text-base
              font-medium
              text-white
              bg-indigo-600
              hover:bg-indigo-700
            "
          >
            Sohbet
          </a>
        </div>
      </div>
    </div>

    <div class="max-w-7xl mx-auto px-4 sm:px-6">
      
<div class="bg-white dark:bg-gray-800 ">
    <div class="lg:flex lg:items-center lg:justify-between w-full mx-auto py-12 px-4 sm:px-6 lg:py-16 lg:px-8 z-20">
        <h2 class="text-3xl font-extrabold text-black dark:text-white sm:text-4xl">
            <span class="block">
                Aşağılık sosyal medya uygulamalarından sıkıldınız mı?
            </span>
            <br>
            <span class="block text-indigo-500">
                Aradığınız şey burada
            </span>
        </h2>
        <div class="lg:mt-0 lg:flex-shrink-0">
            <div class="ml-3 inline-flex rounded-md shadow">
            </div>
            <div class=" inline-flex rounded-md shadow">
            </div>
        </div>
    </div>
</div>

    </div> 
</template>
<script>
    export default ({
        components: {
        },
    })
</script>
