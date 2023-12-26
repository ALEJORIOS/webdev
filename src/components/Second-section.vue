<script setup lang='ts'>
</script>

<template>
    <div class="section-two">
        <h1 class="title">Servicios</h1>
        <div class="service">
            <div class="title">
                Diseñamos o rediseñamos tus páginas y aplicaciones web
            </div>
            <div class="description">
            </div>
        </div>
    </div>
</template>

<style>
.section-two {
    background: linear-gradient(150deg, #0a001b 70%, #0d366e80);
    background-color: #0a001b;
    height: 100dvh;
    padding: 20px;
    display: flex;
    flex-direction: column;
    align-items: center;
    box-sizing: border-box;
    & .title {
        color: white;
        margin: 0;
        margin-bottom: 24px;
    }
    & .service {
        border: 1px solid #fff;
        border-radius: 36px;
        box-shadow: 4px 4px 0 0 #0f0037;
        padding: 24px;
        & .title {
            font-weight: 500;
            font-size: 24px;
        }
        & .description {
            
        }
    }
}
</style>