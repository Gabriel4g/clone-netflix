<template>
    <section id="section-profile">
        <div id="content-profile">
            <div class="info-profile">
                <h1>Crie perfis para crianças.</h1>
                <h2>
                  Deixe as crianças se aventurarem com seus personagens favoritos em um espaço feito 
                  só para elas, sem pagar a mais por isso.  
                </h2>
            </div>

            <img src="../assets/profile-kids.png" alt="Image">
        </div>
    </section>
</template>

<style scoped>
    section#section-profile {
        display: flex;
        justify-content: center;
        padding: 7rem 4.5rem;
        margin-bottom: 1rem;
        background: #000;
    }

    section#section-profile #content-profile {
        display: flex;
        align-items: center;
        gap: 5rem;
    }

    section#section-profile #content-profile > .info-profile {
        display: flex;
        flex-direction: column;
        gap: 2rem;
    }

    section#section-profile #content-profile > .info-profile h1 {
        font-size: 5rem;
        font-family: 'Inter', sans-serif;
        font-weight: 600;
        color: #fff;
        max-width: 50rem;
    }

    section#section-profile #content-profile > .info-profile h2 {
        font-size: 2.6rem;
        font-family: 'Inter', sans-serif;
        font-weight: 500;
        color: #fff;
        max-width: 60rem;
    }

    section#section-profile #content-profile img {
        width: 46.3rem;
    }

    @media screen and (max-width: 1100px) {
        section#section-profile #content-profile {
            flex-direction: column;
        }

        section#section-profile #content-profile > .info-profile h1 {
            font-size: 4rem;
            text-align: center;
            max-width: 100%;
        }

        section#section-profile #content-profile > .info-profile h2 {
            font-size: 2rem;
            max-width: 100%;
            text-align: center;
        }
    }

    @media screen and (max-width: 550px) {
        section#section-profile #content-profile > .info-profile h1 {
            font-size: 2.6rem;
        }

        section#section-profile #content-profile > .info-profile h2 {
            font-size: 1.8rem;
        }

        section#section-profile #content-profile img {
            width: 100%;
        }
    }
</style>

<script>
</script>