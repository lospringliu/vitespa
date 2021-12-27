<script setup lang="ts">
</script>

<template>
  <div class="relative min-h-[712px] max-w-[350px] mx-auto sm:h-[712px] sm:w-[350px] sm:bg-black sm:rounded-[60px] shadow-xl overflow-hidden border-x-[1px] sm:border-[14px] border-black">
    <img src="/pic.jpg" class="absolute inset-0 h-full w-full object-cover" alt="backgroud picture" />
    <div class="invisible absolute top-0 inset-0 sm:visible">
      <div class="h-6 w-40 mx-auto bg-black rounded-b-3xl"></div>
    </div>
    <div class="invisible relative mt-2 mr-5 flex justify-end space-x-1 sm:visible">
      <carbon-dicom-overlay class="h-4 w-4" />
      <carbon-language class="h-4 w-4" />
      <carbon-scooter class="h-4 w-4" />
    </div>
    <div class="invisible relative mt-1.5 h-0.5 w-10 bg-white mr-7 ml-auto sm:visible"></div>
    <div class="relative mt-2 flex flex-col items-center">
      <mdi-lock class="text-white h-8 w-8" />
      <p class="mt-3 text-white text-6xl font-extralight">
        9:41
      </p>
      <p class="mt-1 text-white text-lg font-extralight">
        Friday, July 7th
      </p>
    </div>
    <div class="relative mt-4 mx-2">
      <div class="absolute -bottom-4 inset-x-0 h-full bg-white/10 backdrop-blur-md rounded-3xl">
      </div>
      <div class="absolute -bottom-2 inset-x-0 h-full bg-white/10 backdrop-blur-md rounded-3xl">
      </div>
      <div class="p-4 bg-white/40 backdrop-blur-md rounded-3xl shadow-sm">
        <div class="flex justify-between">
          <div>
            <p class="text-xs font-bold">
              9:30 AM
            </p>
            <h2 class="text-lg font-bold">
              Your Morning Summary
            </h2>
          </div>
          <span class="bg-green-500 rounded-full h-8 w-8 text-white flex items-center justify-center">
            11
          </span>
        </div>
        <div class="mt-2 grid grid-cols-2 gap-2">
          <div>
            <img src="/cova.png" class="rlounded-lg" alt="covide vacine" />
            <h3 class="mt-2 text-xs font-bold leading-tight">
              Surfing: heals the soul, kills the ribs.
            </h3>
            <p class="mt-1 text-xs">
              Itis all fun and thrills until you get sucked over the falls.
            </p>
          </div>
          <div>
            <img src="/cova.png" class="rlounded-lg" alt="covide vacine" />
            <h3 class="mt-2 text-xs font-bold leading-tight">
              Surfing: heals the soul, kills the ribs.
            </h3>
            <p class="mt-1 text-xs">
              Itis all fun and thrills until you get sucked over the falls.
            </p>
          </div>
        </div>
        <hr class="mt-4 border-black/20" />
        <div class="mt-3 grid grid-cols-3 gap-1 items-end">
          <div class="col-span-2">
            <h3 class="text-sm font-bold">
              More Updates
            </h3>
            <p class="mt-05 text-xs">
              hello world blabla ...
            </p>
          </div>
          <ul class="flex flex-row-reverse -space-x-4 space-x-reverse">
            <li><img src="/t.png" alt="" class="h-8 w-8 object-cover rounded-xl" /></li>
            <li><img src="/u.png" alt="" class="h-8 w-8 object-cover rounded-xl" /></li>
            <li><img src="/v.png" alt="" class="h-8 w-8 object-cover rounded-xl" /></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="absolute bottom-0 inset-x-0 h-20">
      <div class="flex justify-between items-center px-10">
        <button class="flex items-center justify-center bg-gray-800/50 backdrop-blur-md rounded-full p-2">
          <mdi-flashlight class="h-6 w-6 text-white" />
        </button>
        <button class="flex items-center justify-center bg-gray-800/50 backdrop-blur-md rounded-full p-2">
          <mdi-camera class="h-6 w-6 text-white" />
        </button>
      </div>
    </div>
    <div class="absolute bottom-1 inset-x-0">
      <div class="mx-auto h-1 w-28 bg-white rounded"></div>
    </div>
  </div>
</template>
