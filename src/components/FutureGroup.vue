<script setup>
    import GradientLine from './GradientLine.vue';
    defineProps({
        title: String,
        msg: String,
    })
</script>

<template>
    <div class="future-item-wrapper">
    <GradientLine/>
    <div class="future-item">
        <h3>{{ title }}</h3>
        <p>{{ msg }}</p>
    </div>
    </div>
</template>

<style scoped>
    .future-item {
        display: flex;
        justify-content: space-between;
        gap: 75px;
    }
    h3 {
        font-size: 18px;
        margin-top: 10px;
        font-weight: 800;
        max-width: 182px;
    }
    p {
        font-size: 14px;
        max-width: 334px;
    }
</style>