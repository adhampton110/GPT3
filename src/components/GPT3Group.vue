<script setup>
import GradientLine from './GradientLine.vue';
defineProps({
    title: String,
    msg: String,
})
</script>

<template>
    <div class="group-item">
        <GradientLine/>
        <h3>{{ title }}</h3>
        <p>{{ msg }}</p>
    </div>  
</template>

<style scoped>
    h3 {
        margin-top: 12px;
    }
</style>