<template>
  <div>
    <div class="grid grid-cols-4 gap-5">
      <div v-for="p in portfolio" v-bind:key="p in portfolio">
        <PortfolioCard :portfolio="p" />
      </div>
    </div>
  </div>
</template>

<script setup>
//  fetch the products
const { data: portfolio } = await useFetch("https://fakestoreapi.com/products");

definePageMeta({
  layout: "portfolio",
});

useHead({
  title: "MiaCodes | Portfolio",
  meta: [{ name: "description", content: "Work Ive done" }],
});
</script>

<style scoped></style>
