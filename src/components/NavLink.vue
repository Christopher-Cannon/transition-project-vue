<script setup>
const { text, link, isButton } = defineProps(['text', 'link', 'isButton']);
</script>

<template>
  <li><a :href="link" class="nav-link" :class="{ btn: isButton }">{{ text }}</a></li>
</template>