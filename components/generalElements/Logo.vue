<script setup>
const runtimeConfig = useRuntimeConfig();
const logoUrl = runtimeConfig?.public?.LOGO || null;
</script>

<template>
  <NuxtLink to="/">
    <img src="https://vincor.com/wp-content/uploads/vincor_media/Artboard-1-copy-2.png" alt="Logo" class=" h-16" />
  </NuxtLink>
</template>
