<template>
  <div class="card text-center">
    <img :src="`${portfolio.image}`" alt="portfolio image" class="thumb" />
    <p class="font-bold text-gray-500 m-4 truncate">{{ portfolio.title }}</p>
    <NuxtLink :to="`/portfolio/${portfolio.id}`">
      <p class="btn my-4">View Details</p>
    </NuxtLink>
  </div>
</template>

<script setup>
const { portfolio } = defineProps(["portfolio"]);
</script>

<style scoped>
.thumb {
  max-height: 120px;
  max-width: 70%;
  margin: 0 auto;
}
</style>
