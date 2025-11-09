<template>
  <UHeader>
    <template #title>
      <img src="/logo.svg" class="h-10 w-auto" >
    </template>

    <template #right>
          <UNavigationMenu
      :items="items"
      color="primary"
      :highlight="true"
      variant="link"
      :ui="{
        linkLabel: 'text-2xl'
      }" />
    </template>

  </UHeader>
</template>

<script setup lang="ts">
import type { NavigationMenuItem } from '@nuxt/ui'

const route = useRoute()

const items = computed<NavigationMenuItem[]>(() => [
  {
    label: 'Wemotion',
    to: '/wemotion',
    active: route.path.startsWith('/wemotion')
  },
  {
    label: 'Programm',
    to: '/programm',
    active: route.path.startsWith('/programm')
  },
  {
    label: 'Galerie',
    to: '/galerie',
    active: route.path.startsWith('/galerie')
  },
])
</script>
