<template>
    <section id="section-watch">
        <div id="content-watch">
            <img src="../assets/watch-devices.png" alt="Watch">

            <div class="info-watch">
                <h1>Assista quando quiser.</h1>
                <h2>Assista no celular, tablet, Smart TV ou notebook sem pagar a mais por isso.</h2>
            </div>
        </div>
    </section>
</template>

<style scoped>
    section#section-watch {
        background: #000;
        display: flex;
        justify-content: center;
        padding: 7rem 4.5rem;
        margin-bottom: 1rem;
    }

    section#section-watch #content-watch {
        display: flex;
        align-items: center;
        gap: 6rem;
    }

    section#section-watch #content-watch > .info-watch {
        display: flex;
        flex-direction: column;
        gap: 2rem;
    }

    section#section-watch #content-watch > .info-watch h1 {
        font-size: 5rem;
        font-family: 'Inter', sans-serif;
        font-weight: 600;
        color: #fff;
        text-align: center;
    }

    section#section-watch #content-watch > .info-watch h2 {
        font-size: 2.6rem;
        font-family: 'Inter', sans-serif;
        font-weight: 500;
        color: #fff;
        max-width: 50rem;
    }

    @media screen and (max-width: 1100px) {
        section#section-watch #content-watch {
            flex-direction: column-reverse;
        }

        section#section-watch #content-watch > .info-watch {
            align-items: center;
        }

        section#section-watch #content-watch > .info-watch h1 {
            font-size: 4rem;
        }

        section#section-watch #content-watch > .info-watch h2 {
            text-align: center;
            font-size: 2rem;
            max-width: 100%;
        }

        section#section-watch #content-watch img {
            width: 100%;
        }
    }

    @media screen and (max-width: 550px) {
        section#section-watch #content-watch > .info-watch h1 {
            font-size: 2.6rem;
        }

        section#section-watch #content-watch > .info-watch h2 {
            font-size: 1.8rem;
        }
    }
</style>

<script>
</script>