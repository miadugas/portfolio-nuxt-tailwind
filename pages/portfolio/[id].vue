<template>
    <div>
        <p>Portfolio Ddetails for {{ id }}</p>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde beatae voluptatum impedit illo sequi ullam quidem temporibus, quod mollitia nihil rerum expedita sit delectus porro atque, natus inventore amet tempora?</p>
    </div>
</template>

<script lang='ts' setup>
    const { id } = useRoute().params
</script>

<style scoped>

</style>