<template>
  <div>
    <Head>
      <Title>Mia Codes | {{ portfolio.title }}</Title>
      <Meta name="description" :content="portfolio.description" />
    </Head>

    <PortfolioDetails :portfolio="portfolio" />
  </div>
</template>

<script setup>
const { id } = useRoute().params;
const uri = "https://fakestoreapi.com/products/" + id;

//  fetch the products
const { data: portfolio } = await useFetch(uri, { key: id });

if (!portfolio.value) {
  throw createError({
    statusCode: 404,
    statusMessage: "Page not found",
    fatal: true,
  });
}

definePageMeta({
  layout: "portfolio",
});
</script>

<style scoped></style>
