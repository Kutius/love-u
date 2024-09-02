<script setup lang="ts">
const avatarLeft = 'https://q1.qlogo.cn/g?b=qq&nk=647159607&s=640'
const avatarRight = 'https://q1.qlogo.cn/g?b=qq&nk=917640289&s=640'
</script>

<template>
  <div
    bg="white op20"
    mx-6 h-50 w-200
    flex items-center justify-center gap-25
    overflow-hidden rounded-3xl backdrop-blur-xl
    shadow="md"
  >
    <div flex="~ col gap-2" cursor-pointer>
      <NuxtImg size-20 rounded-full :src="avatarLeft" loading="lazy" />
      <span text-xl>Yun</span>
    </div>

    <div
      size-20 flex select-none items-center justify-center text-12
      class="animated"
    >
      ❤️
    </div>

    <div flex="~ col gap-2" cursor-pointer>
      <NuxtImg size-20 rounded-full :src="avatarRight" loading="lazy" />
      <span text-xl>Hammer</span>
    </div>
  </div>
</template>

<style scoped>
.animated {
  /* scale animation */
  animation: scale 1s infinite;
}

@keyframes scale {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.2);
  }
  100% {
    transform: scale(1);
  }
}
</style>
