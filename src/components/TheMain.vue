<script>
const inputEmail = document.querySelector("#email-input");
const buttonSendEmail = document.querySelector("#btn-started");

export default {
    name: "TheMain",
    methods: {
        checkInput: (e) => {
            e.preventDefault();

            if(!inputEmail.value.includes("@")) {
                alert("Coloque o @")
            }
        }
    }
}

</script>

<template>
  <main>
    <header>
      <div id="content-header">
        <svg
          viewBox="0 0 111 30"
          data-uia="netflix-logo"
          class="svg-icon svg-icon-netflix-logo"
          aria-hidden="true"
          focusable="false"
          width="150"
          fill="red"
        >
          <g id="netflix-logo">
            <path
              d="M105.06233,14.2806261 L110.999156,30 C109.249227,29.7497422 107.500234,29.4366857 105.718437,29.1554972 L102.374168,20.4686475 L98.9371075,28.4375293 C97.2499766,28.1563408 95.5928391,28.061674 93.9057081,27.8432843 L99.9372012,14.0931671 L94.4680851,-5.68434189e-14 L99.5313525,-5.68434189e-14 L102.593495,7.87421502 L105.874965,-5.68434189e-14 L110.999156,-5.68434189e-14 L105.06233,14.2806261 Z M90.4686475,-5.68434189e-14 L85.8749649,-5.68434189e-14 L85.8749649,27.2499766 C87.3746368,27.3437061 88.9371075,27.4055675 90.4686475,27.5930265 L90.4686475,-5.68434189e-14 Z M81.9055207,26.93692 C77.7186241,26.6557316 73.5307901,26.4064111 69.250164,26.3117443 L69.250164,-5.68434189e-14 L73.9366389,-5.68434189e-14 L73.9366389,21.8745899 C76.6248008,21.9373887 79.3120255,22.1557784 81.9055207,22.2804387 L81.9055207,26.93692 Z M64.2496954,10.6561065 L64.2496954,15.3435186 L57.8442216,15.3435186 L57.8442216,25.9996251 L53.2186709,25.9996251 L53.2186709,-5.68434189e-14 L66.3436123,-5.68434189e-14 L66.3436123,4.68741213 L57.8442216,4.68741213 L57.8442216,10.6561065 L64.2496954,10.6561065 Z M45.3435186,4.68741213 L45.3435186,26.2498828 C43.7810479,26.2498828 42.1876465,26.2498828 40.6561065,26.3117443 L40.6561065,4.68741213 L35.8121661,4.68741213 L35.8121661,-5.68434189e-14 L50.2183897,-5.68434189e-14 L50.2183897,4.68741213 L45.3435186,4.68741213 Z M30.749836,15.5928391 C28.687787,15.5928391 26.2498828,15.5928391 24.4999531,15.6875059 L24.4999531,22.6562939 C27.2499766,22.4678976 30,22.2495079 32.7809542,22.1557784 L32.7809542,26.6557316 L19.812541,27.6876933 L19.812541,-5.68434189e-14 L32.7809542,-5.68434189e-14 L32.7809542,4.68741213 L24.4999531,4.68741213 L24.4999531,10.9991564 C26.3126816,10.9991564 29.0936358,10.9054269 30.749836,10.9054269 L30.749836,15.5928391 Z M4.78114163,12.9684132 L4.78114163,29.3429562 C3.09401069,29.5313525 1.59340144,29.7497422 0,30 L0,-5.68434189e-14 L4.4690224,-5.68434189e-14 L10.562377,17.0315868 L10.562377,-5.68434189e-14 L15.2497891,-5.68434189e-14 L15.2497891,28.061674 C13.5935889,28.3437998 11.906458,28.4375293 10.1246602,28.6868498 L4.78114163,12.9684132 Z"
              id="Fill-14"
            ></path>
          </g>
        </svg>

        <div class="info-header">
          <select id="language">
            <option value="Português">Português</option>
            <option value="English">English</option>
          </select>

          <button id="btn-sign">Entrar</button>
        </div>
      </div>
    </header>

    <div id="content-main">
      <h1>
        Filmes, séries e muito mais.
        Sem Limites.
      </h1>

      <h2>Assista onde quiser. Cancele quando quiser.</h2>

      <form action="">
        <p>
          Pronto para assistir? Informe seu email para criar ou reiniciar sua
          assinatura.
        </p>

        <div id="content-sign">
          <input type="email" id="email-input" placeholder="Email" />
          <button id="btn-started" @click="checkInput">
            Vamos lá
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="icon icon-tabler icon-tabler-arrow-right"
              width="28"
              height="28"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="#fff"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <path stroke="none" d="M0 0h24v24H0z" fill="none" />
              <line x1="5" y1="12" x2="19" y2="12" />
              <line x1="13" y1="18" x2="19" y2="12" />
              <line x1="13" y1="6" x2="19" y2="12" />
            </svg>
          </button>
        </div>
      </form>
    </div>
  </main>
</template>

<style>
main {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 14rem;
  background-image: url(../assets/background-films.jpg);
  background-size: cover;
  background-position: center;
  background-blend-mode: color;
  background-color: rgb(0, 0, 0, 0.6);
  height: 70rem;
  margin-bottom: 1rem;
}

main header {
  padding: 3rem 0 0;
  width: 100%;
  display: flex;
  justify-content: center;
}

main header > #content-header {
  width: 90%;
  max-width: 1500px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

main header > #content-header .info-header {
  display: flex;
  gap: 2rem;
  align-items: center;
}

main header > #content-header select {
  padding: 0.8rem 1rem;
  font-size: 1.5rem;
  background: none;
  color: #fff;
  font-family: "Poppins", sans-serif;
}

main header > #content-header select > option {
  color: #000;
  font-size: inherit;
}

main header > #content-header button#btn-sign {
  padding: 0.7rem 1.7rem;
  font-size: 1.6rem;
  background: #e50914;
  color: #fff;
  font-family: "Inter", sans-serif;
  border: none;
  border-radius: 0.3rem;
  font-weight: 500;
  cursor: pointer;
}

main #content-main {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
}

main #content-main h1 {
  text-align: center;
  font-size: 5rem;
  font-family: "Inter", sans-serif;
  color: #fff;
  font-weight: 600;
  width: 70%;
}

main #content-main h2 {
  font-size: 2.6rem;
  font-family: "Inter", sans-serif;
  font-weight: 500;
  color: #fff;
  margin-bottom: 1rem;
  text-align: center;
}

main #content-main > form {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
}

main #content-main > form p {
  font-size: 2rem;
  font-family: "Inter", sans-serif;
  color: #fff;
  text-align: center;
}

main #content-main > form > #content-sign {
  display: flex;
  justify-content: center;
}

main #content-main > form > #content-sign input {
  width: 50rem;
  font-size: 1.6rem;
  padding: 1rem;
  height: 6rem;
  outline: none;
}

main #content-main > form > #content-sign button {
  background: #e50914;
  color: #fff;
  border: none;
  cursor: pointer;
  width: 18.3rem;
  font-size: 2.6rem;
  font-family: 'Inter', sans-serif;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;
}



@media screen and (max-width: 950px) {
    main header #content-header > svg {
        width: 10rem;
    }

    main #content-main > form > #content-sign {
        width: 90%;
        flex-direction: column;
        align-items: center;
        gap: 1.5rem;
    }

    main #content-main > form p {
        font-size: 2.3rem;
        max-width: 50rem;
    }

    main #content-main > form > #content-sign input {
        width: 100%;
    }

    main #content-main > form > #content-sign button {
        padding: 1rem;
        border-radius: 5px;
    }
}

@media screen and (max-width: 750px) {
    main {
      height: 785px;
    }

    main {
        background-color: rgb(0, 0, 0, 0.5);
    }

    main #content-main h1 {
      width: 90%;
    }

    main #content-main > form > p {
        font-size: 1.8rem;
    }

    main #content-main > form #content-sign > input {
      font-size: 1.4rem;
    }
}

@media screen and (max-width: 550px) {
    main {
      height: 600px;
      gap: 8rem;
    }

    main header #content-header select {
        padding: 0.2rem;
    }

    main #content-main h1 {
        font-size: 2.8rem;
        width: 80%;
    }

    main #content-main h2 {
        font-size: 1.8rem;
        width: 60%;
    }

    main #content-main p {
      width: 90%;
    }

    main #content-main form > #content-sign > button {
      font-size: 1.6rem;
      width: 13rem;
    }
}
</style>