<template>
  <a class="featuredCategory" :class="class" :href="link">
    <img :src="img" :alt="imgAlt" class="block m-auto mb-5 w-4/6 max-w-xs h-auto" />
    <p class="title uppercase font-semibold text-center">
      {{ title }}
    </p>
    <p class="subtitle text-slate-500 text-center m-auto">
      {{ subtitle }}
    </p>
  </a>
</template>

<script setup lang="ts">
defineProps(['link', 'img', 'imgAlt', 'title', 'subtitle', 'class']);
</script>