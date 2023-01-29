<template>
  <div class="marquee-horizontal whitespace-nowrap overflow-hidden">
    <h2 class="text-8xl whitespace-nowrap my-16 inline-block font-semibold" v-for="x in 4">
      A <span class="text-outline">Reusable</span> Way of Living. &nbsp;
    </h2>
  </div>
</template>

<script setup lang="ts">
</script>

<style lang="scss" scoped>
@keyframes slideLeft {
  from {
    transform: translateX(0);
  }

  to {
    transform: translateX(-100%);
  }
}

.marquee-horizontal {
  h2 {
    animation-name: slideLeft;
    animation-duration: 10s;
    animation-timing-function: linear;
    animation-iteration-count: infinite;
  }
}
</style>