<script setup>
const { item } = defineProps(['item']);
const { image, heading, description, subtitle, arrow, inverted } = item;
</script>

<template>
  <a href="#" class="news-item" :class="{ 'news-item-inverted': inverted }">
    <img :src="image" alt="" class="news-item-image" />

    <div class="news-item-info">
      <h2 class="news-item-heading">
        {{ heading }}
      </h2>

      <p>{{ description }}</p>

      <p class="news-item-subtitle">
        <strong>{{ subtitle }}</strong>
      </p>

      <div class="news-item-arrow">
        <img :src="arrow" alt="" />
      </div>
    </div>
  </a>
</template>
