<script setup>
    import FooterData from '../../data/FooterData.json';
</script>
<template>
    <footer>
        <div class="flex-wrapper">
            <div>
                <img src="../../assets/logo.svg" alt="logo">
                <p style="width:168px" class="content">Crechterwoord K12 182 DK Alknjkcb, All Rights Reserved</p>
            </div>
            <div class="item-wrapper">
                <div class="item" v-for="obj in FooterData">
                    <p class="title">{{ obj.title }}</p>
                    <a href="#" class="content" v-for="link in obj.links">{{ link }}</a>
                </div>
            </div>
        </div>
        <p style="padding-bottom: 14px;" class="content">© 2021 GPT-3 All rights reserved.</p>
    </footer>
</template>

<style scoped>
    * {
        color: #FFFFFF;
    }
    .flex-wrapper {
        display: flex;
        justify-content: space-around;
        margin-bottom: 80px;
    }
    .title {
        font-size: 14px;
        font-weight: 700;
    }
    .content {
        font-size: 14px;
        text-decoration: none;
    }
    .item-wrapper {
        display: flex;
        gap: 160px;
    }
    .item {
        display: flex;
        flex-direction: column;
        gap:20px;
    }
</style>