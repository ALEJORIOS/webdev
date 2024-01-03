<script setup lang='ts'>
</script>

<template>
    <section class="section-three">
        <div class="text">
            <span>Construimos las mejores soluciones</span>
            <span>con la mejor tecnología</span>
        </div>
    </section>
</template>

<style>

.section-three { 
    height: 300dvh;
    position: relative;
    padding-top: 10vmin;
    background-color: #0a001b;
    
    & .text {
        position: sticky;
        height: fit-content;
        top: 40%;
        display: flex;
        flex-direction: column;
        font-size: 6vmin;
        font-weight: 800;
        color: #c500cc;
        justify-content: center;
        align-items: center;
        view-timeline: --colorTimeline;
        animation-timeline: --colorTimeline;
        animation-name: changeColor;
        animation-duration: 1ms;
        animation-range: contain cover;
        & .emphasis {
            color: red;
        }
    }
    
}

@keyframes changeColor {
    0% {
        color: #c500cc;
    }
    50% {
        color: #0796d3;
    }

    99% {
        color: #c500cc;
    }
}

</style>