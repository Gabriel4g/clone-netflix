<template>
  <section id="section-watch">
    <div class="info-watch">
      <h1>Aproveite na TV.</h1>
      <h2>
        Assista em Smart TVs, PlayStation, Xbox, Chromecast, Apple TV, aparelhos
        de Blu-ray e outros dispositivos.
      </h2>
    </div>

    <img src="../assets/watch.png" alt="Watch TV" />
  </section>
</template>

<style scoped>
section#section-watch {
  display: flex;
  justify-content: center;
  align-items: center;
  background: #000000;
  gap: 2rem;
  padding: 7rem 4.5rem;
  margin-bottom: 1rem;
}

section#section-watch .info-watch {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    color: #fff;
}

section#section-watch .info-watch h1 {
    font-size: 5rem;
    font-family: 'Inter', sans-serif;
    font-weight: 600;
}

section#section-watch .info-watch h2 {
    font-size: 2.6rem;
    font-family: 'Inter', sans-serif;
    font-weight: 500;
    max-width: 58rem;
}

@media  screen and (max-width: 1100px) {
    section#section-watch {
        flex-direction: column;
    }

    section#section-watch .info-watch {
        text-align: center;
    }

     section#section-watch .info-watch h1 {
         font-size: 4rem;
     }

    section#section-watch .info-watch h2 {
        max-width: 80rem;
        font-size: 2rem;
    }
}

@media  screen and (max-width: 630px) {
    section#section-watch img {
        width: 100%;
    }

     section#section-watch .info-watch h1 {
         font-size: 2.6rem;
     }

      section#section-watch .info-watch h2 {
          font-size: 1.8rem;
      }
}
</style>

<script>
</script>