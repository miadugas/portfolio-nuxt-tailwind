<template>
  <div>
    <p>Portfolio Details for {{ id }}</p>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde beatae
      voluptatum impedit illo sequi ullam quidem temporibus, quod mollitia nihil
      rerum expedita sit delectus porro atque, natus inventore amet tempora?
    </p>
  </div>
</template>

<script setup>
const { id } = useRoute().params

definePageMeta({
    layout: "portfolio"
});
</script>

<style scoped></style>
