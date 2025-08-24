<script setup>
    
</script>

<template>
  <header class="h-[373px]">
      <img src="/bg-mobile.svg" alt="bg-mobile" class="absolute z-[-10]">
      <div class="flex flex-col px-7 items-start pt-6 gap-12">
        <img src="/logo.svg" alt="bg-mobile" class="h-10">
        <img src="/illustration-mockups.svg" alt="bg-mobile" class="z-10">
      </div>
  </header>
  <body class="flex flex-col flex-1">
    <slot/>
  </body>
  <footer class="flex flex-col gap-5">
    <div class="flex justify-center gap-2">
      <button class="text-md border-white border-1 rounded-full h-8 aspect-[1/1] text-white">
          <i class="fa-brands fa-facebook-f"></i>
      </button>
      <button class="text-md border-white border-1 rounded-full h-8 aspect-[1/1] text-white">
          <i class="fa-brands fa-twitter"></i>
      </button>
      <button class="text-md border-white border-1 rounded-full h-8 aspect-[1/1] text-white">
          <i class="fa-brands fa-instagram"></i>
      </button>
    </div>
    <p class="attribution">
      Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
      Coded by <a href="#">Hazerin</a>.
    </p>
  </footer>
</template>

<style scoped>

</style>
