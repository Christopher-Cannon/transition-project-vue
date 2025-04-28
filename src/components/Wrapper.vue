<script setup>
const { classes } = defineProps(['classes']);
</script>

<template>
  <div class="page-wrapper" :class="{ [classes]: classes}">
    <slot />
  </div>
</template>