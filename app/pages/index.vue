<script setup lang="ts">
const bgLink = 'https://dagvqwfczlevrtjztrvr.supabase.co/storage/v1/object/public/imgs/hero.jpg'
</script>

<template>
  <div relative h-150 flex items-center justify-center>
    <Hearter />

    <NuxtImg
      class="absolute left-0 top-0 z--1 h-full w-full"
      object-cover filter-brightness-80
      loading="lazy"
      :src="bgLink"
    />
  </div>
</template>
