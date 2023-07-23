<script setup>
    defineProps({
        date: String,
        title: String,
        imageName: String,
        size: String,
    });
</script>

<template>
    <div class="card">
        
        <img src="../assets/blog01.png" v-bind:alt="imageName" >
        <div class="card-content">
            <div>
                <p>{{ date }}</p>
            <h3>{{ title }}</h3>
            </div>
            
            <p>Read Full Article</p>
        </div>
        
    </div>
</template>

<style scoped>
    .card {
        display: flex;
        flex-direction: column;
        width: 420px;
    }
    .card * {
        color: white;
        line-height: 30.287px;
    }
    img {
        height: 130px;
    }
    .card-content {
        background-color: #042C54;
        height: 194px;
        justify-content: space-between;
        display: flex;
        flex-direction: column;
        padding: 16px;
    }
    p {
        font-weight: 700;

    }
</style>