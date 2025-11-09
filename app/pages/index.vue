<template>
  <UContainer class="grow flex flex-col justify-center items-center gap-20">
    <img src="/logo.svg" alt="Logo" class="h-40" >
    <div class="text-white text-3xl font-bold">
      Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.
    </div>
    <div class="grid grid-cols-3 w-full">
      <div class="flex">
        <NuxtLink to="/wemotion">
          <img src="/menu_wemotion.svg" >
        </NuxtLink>
      </div>
      <div class="flex justify-center">
        <NuxtLink to="/programm" class="mx-auto">
          <img src="/menu_programm.svg" >
        </NuxtLink>
      </div>
      <div class="flex justify-end">
        <NuxtLink to="/galerie">
          <img src="/menu_galerie.svg" >
        </NuxtLink>
      </div>
    </div>
  </UContainer>
</template>
<script setup lang="ts">

definePageMeta({
  layout: 'landing',
})
</script>
