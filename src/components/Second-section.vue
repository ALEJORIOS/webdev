<script setup lang='ts'>
</script>

<template>
    <div class="section-two">
        <div class="header">
            <h1 class="title">Servicios</h1>
        </div>
        <div class="service">
            <div class="title">
                <i class="fa-solid fa-pencil"></i>
                Diseño de páginas y aplicaciones web
            </div>
            <p class="description">
                Nos enfocamos en desarrollar interfaces atractivas y funcionales que reflejen fielmente la identidad que deseas proyectar, asegurando así que cada interacción con tu sitio web o aplicación sea memorable y eficaz para tu audiencia.
            </p>
        </div>

        <div class="service">
            <div class="title">
                <i class="fa-solid fa-store"></i>
                Tiendas virtuales
            </div>
            <p class="description">
                ¿Deseas llevar tus productos al <b>mundo digital</b>? nosotros te ayudamos desarrollando una <b>tienda virtual</b> adaptada completamente a tus necesidades brindandote una solución integral para que puedas ofrecer tus productos con confianza y comodidad en línea.
            </p>
        </div>
        <div class="service">
            <div class="title">
                <i class="fa-solid fa-desktop"></i>
                Desarrollo de aplicaciones para escritorio
            </div>
            <p class="description">
                ¿Necesitas una solución sin necesidad de conectarse a internet? Desarrollamos aplicaciones para escritorio, tanto en <b>Windows</b> como en <b>Mac</b>, que pueden funcionar sin necesidad de una conexión constante a internet.
            </p>
        </div>
        <div class="service">
            <div class="title">
                <i class="fa-solid fa-mobile-screen-button"></i>
                Desarrollo de aplicaciones móviles
            </div>
            <p class="description">
                ¿Piensas en una solución enfocada en dispossitivos móviles? Claro que sí, creamos aplicaciones móviles para <b>Android/iOS</b>, ya sea para uso privado o para su distribución en las tiendas (Play Store/App Store).
            </p>
        </div>
        <div class="more">Muchos más</div>
    </div>
</template>

<style>
.section-two {
    background: linear-gradient(150deg, #0a001b 70%, #0d366e80);
    background-color: #0a001b;
    height: 100dvh;
    padding: 20px;
    display: grid;
    box-sizing: border-box;
    grid-template-columns: repeat(2, 30dvw);
    grid-template-rows: auto repeat(2, auto) auto;
    column-gap: 1vw;
    row-gap: 1vw;
    justify-content: center;
    & > .header {
        display: flex;
        color: white;
        margin: 0;
        grid-column: 1 / 3;
        justify-content: center;
        & h1 {
            margin-bottom: 0;
            text-shadow: 0 0 8px #9b31db;
        }
    }
    & .service {
        /* border: 1px solid #fff; */
        border: 2px solid rgba(255, 255, 255, 0.422);
        background-color: #0F003750;
        backdrop-filter: blur(10px);
        border-radius: 36px;
        box-shadow: 4px 4px 0 0 #0f0037;
        padding: 36px;
        & .title {
            font-weight: 500;
            font-size: 24px;
            color: #9b31db;
            text-shadow: 0 0 6px #9b31dbaa;
        }
        & .description {
            color: white;
            /* text-align: justify; */
            /* text-justify: inter-character; */
            font-size: 16px;
            line-height: 22px;
            & b {
                text-shadow: 0 0 4px #9b31db;
            }
        }
    }

    & .more {
        grid-column: 1/-1;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 28px;
        color: #fff;
        background: linear-gradient(-20deg, #0d366e 0%, #6916cd 50%, #c500cc 100%);
        height: 6vmax;
        border: none;
        box-shadow: none;
        border-radius: 4vmax;
        flex-direction: row;
        cursor: pointer;
        text-shadow: 0 0 10px #ebc9ff;
        user-select: none;
    }
}
</style>