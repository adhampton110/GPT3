<script setup>
defineProps({
    title: String,
    msg: String,
})
</script>

<template>
    <h3>{{ title }}</h3>
    <p>{{ msg }}</p>
</template>

<style scoped>
</style>