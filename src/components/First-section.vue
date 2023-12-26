<script setup lang='ts'>
import Stars from './Stars.vue';
import { onMounted, ref } from 'vue';

let loaded = ref(false)
onMounted(() => {
    loaded.value = true;
});
</script>

<template>
    <div class="section-one">
        <div class="stars">
            <Stars/>
        </div>
        <Transition>
            <div v-if="loaded" class="textContent">
                <span class="rivers-grove">Rivers Grove</span>
                <span class="webdev">Web dev</span>
                <span class="text">Convertimos tus ideas en <br> <span>experiencias digitales</span></span>
            </div>
        </Transition>
        <div class="bottom"></div>
    </div>
</template>

<style>
.section-one {
    & .textContent {
        position: absolute;
        top: 0;
        left: 10dvw;
        flex-direction: column;
        height: 100dvh;
        display: flex;
        justify-content: center;
        overflow: hidden;
        & .rivers-grove {
            font-size: clamp(20px, 15px + 2vw, 30vw);
            font-weight: 800;
            color: #4700c1;
        }

        & .webdev {
            font-size: clamp(60px, 45px + 6vw, 30vw);
            line-height: clamp(60px, 35px + 6vw, 30vw);
            font-weight: 800;
            color: #d3d3e9;
        }

        & .text {
            font-size: clamp(15px, 12px + 2vw, 30vw);
            font-weight: 600;
            color: #d3d3e9;
            user-select: none;
            & span {
                font-weight: 700;
                color: #6f1bff;
                line-height: clamp(15px, 12px + 2vw, 30vw);
                transition: font-size 1s;
                &:hover {
                    font-size: clamp(15px, 16px + 2vw, 30vw);
                    transition: font-size 1s;
                    cursor: pointer;
                }
            }
        }
    }
}
.section-one .bottom {
    position: absolute;
    bottom: 0;
    width: 100%;
    height: 25dvh;
    background: linear-gradient(transparent, black 50%, #0a001b);
}
</style>