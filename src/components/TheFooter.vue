<template>
  <footer>
    <div id="content-footer">
      <p class="phone">Dúvidas? Ligue <a href="#">0800 591 8942</a></p>

      <div id="content-links-footer">
        <div class="group-footer">
          <a class="link-footer" href="#">Perguntas frequentes</a>
          <a class="link-footer" href="#">Relações com investidores</a>
          <a class="link-footer" href="#">Formas de assistir</a>
          <a class="link-footer" href="#">Informações corporativas</a>
          <a class="link-footer" href="#">Só na netflix</a>
        </div>

        <div class="group-footer">
          <a class="link-footer" href="#">Central de ajuda</a>
          <a class="link-footer" href="#">Carreiras</a>
          <a class="link-footer" href="#">Termos de Uso</a>
          <a class="link-footer" href="#">Entre em contato</a>
        </div>

        <div class="group-footer">
          <a class="link-footer" href="#">Conta</a>
          <a class="link-footer" href="#">Resgatar cartão pré-pago</a>
          <a class="link-footer" href="#">Privacidade</a>
          <a class="link-footer" href="#">Teste de velocidade</a>
        </div>

        <div class="group-footer">
          <a class="link-footer" href="#">Media Center</a>
          <a class="link-footer" href="#">Comprar cartão pré-pago</a>
          <a class="link-footer" href="#">Preferências de cookies</a>
          <a class="link-footer" href="#">Avisos legais</a>
        </div>
      </div>

      <div class="language-content">
        <select id="select-language" @change="changeTextLanguage">
          <option value="Português">Português</option>
          <option value="English">English</option>
        </select>

        <p class="footer-country">Netflix Brasil</p>
      </div>
    </div>
  </footer>
</template>

<style scoped>
    footer {
        padding: 7rem 4.5rem;
        background: #000;
    }

    footer #content-footer {
        width: 100%;
        display: flex;
        flex-direction: column;
        gap: 4rem;
        align-items: center;
    }

    footer #content-footer > p.phone {
        font-size: 1.6rem;
        font-family: 'Poppins', sans-serif;
        color: #737373;
    }

    footer #content-footer > p.phone > a {
        font-size: inherit;
        font-family: inherit;
        color: inherit;
        text-decoration: none;
    }

    footer #content-footer > p.phone > a:hover {
        text-decoration: underline;
    }

    footer #content-footer > #content-links-footer {
        width: 100%;
        max-width: 900px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }

    footer #content-footer > #content-links-footer > .group-footer {
        display: flex;
        flex-direction: column;
        gap: 2rem;
    }

    footer #content-footer > #content-links-footer > .group-footer a {
        font-size: 1.3rem;
        font-family: 'Inter', sans-serif;
        color: #737373;
        text-decoration: none;
    }

    footer #content-footer > #content-links-footer > .group-footer a:hover {
        text-decoration: underline;
    }

    footer #content-footer > .language-content {
        display: flex;
        flex-direction: column;
        gap: 2rem;
        align-items: center;
    }

    footer #content-footer > .language-content select {
        font-size: 1.6rem;
        font-family: 'Poppins', sans-serif;
        background: none;
        border: none;
        border: 1px solid rgba(92, 87, 87, 0.582);
        color: #fff;
        padding: 1.2rem 2.6rem 1.2rem 5rem;
    }

    footer #content-footer > .language-content select > option {
        font-size: inherit;
        font-family: inherit;
        color: #000;
    }

    footer #content-footer > .language-content p {
        font-size: 1.3rem;
        font-family: 'Inter', sans-serif;
        color: #737373;
    }

    @media screen and (max-width: 710px) {
        footer #content-footer {
            width: 80%;
            align-items: flex-start;
        }

        footer #content-footer > #content-links-footer {
            width: 300px;
            justify-content: flex-start;
            gap: 3rem;
        }
    }

    @media screen and (max-width: 365px) {
        footer #content-footer > #content-links-footer {
            width: 100%;
        }
    }
</style>

<script>
</script>