<template>
    <section id="section-download-series">
        <div id="content-series">
            <img src="../assets/download-series.jpg" alt="Image">

            <div class="info-series">
                <h1>Baixe séries para assistir offline.</h1>
                <h2>Disponível em todos os planos, exceto no Básico com anúncios.</h2>
            </div>
        </div>
    </section>
</template>

<style scoped>
    section#section-download-series {
        display: flex;
        justify-content: center;
        padding: 7rem 4.5rem;
        margin-bottom: 1rem;
        background: #000;
    }

    section#section-download-series #content-series {
        display: flex;
        align-items: center;
        gap: 15rem;
    }

    section#section-download-series #content-series img {
        width: 50rem;
    }

    section#section-download-series #content-series > .info-series {
        display: flex;
        flex-direction: column;
        gap: 2rem;
    }

    section#section-download-series #content-series > .info-series h1 {
        font-size: 5rem;
        font-family: 'Inter', sans-serif;
        font-weight: 600;
        color: #fff;
        max-width: 50rem;
        margin-right: 15rem;
    }

    section#section-download-series #content-series > .info-series h2 {
        font-size: 2.6rem;
        font-family: 'Inter', sans-serif;
        font-weight: 500;
        color: #fff;
        max-width: 50rem;
    }

    @media screen and (max-width: 1320px) {
        section#section-download-series #content-series > .info-series h1 {
            margin: 0;
            max-width: 100%;
        }
    }

    @media screen and (max-width: 1100px) {
        section#section-download-series #content-series {
            flex-direction: column-reverse;
            gap: 2rem;
            text-align: center;
        }

        section#section-download-series #content-series > .info-series h1 {
            font-size: 4rem;
        }

        section#section-download-series #content-series > .info-series h2 {
            max-width: 100%;
            font-size: 2rem;
        }
    }

    @media screen and (max-width: 550px) {
        section#section-download-series #content-series > .info-series h1 {
            font-size: 2.6rem;
        }

        section#section-download-series #content-series > .info-series h2 {
            font-size: 1.8rem;
        }
        section#section-download-series #content-series img {
            width: 100%;
        }
    }
</style>

<script>
</script>