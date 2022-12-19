<script>
</script>

<template>
  <div id="content-promotion">
    <div class="info-promotion">
      <span>NOVO!</span>
      <p>
        Planos a partir de
        <strong> R$18,90. </strong>
      </p>

      <a href="#">
        SaIba MaIs
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="button-icon icon-chevron-next"
        >
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M7.29297 19.2928L14.5859 12L7.29297 4.70706L8.70718 3.29285L16.7072 11.2928C16.8947 11.4804 17.0001 11.7347 17.0001 12C17.0001 12.2652 16.8947 12.5195 16.7072 12.7071L8.70718 20.7071L7.29297 19.2928Z"
            fill="currentColor"
          ></path>
        </svg>
      </a>
    </div>
  </div>
</template>

<style scoped>
#content-promotion {
  height: 6.6rem;
  width: 100%;
  background: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
}

#content-promotion > .info-promotion {
  display: flex;
  gap: 2rem;
  align-items: center;
}

#content-promotion > .info-promotion span {
  font-size: 1.3rem;
  font-weight: 600;
  font-family: "Roboto", sans-serif;
  padding: 3.2px 8px;
  border-radius: 5rem;
  background: #e50914;
  color: #fff;
}

#content-promotion > .info-promotion p {
  font-size: 1.8rem;
  font-family: "Inter", sans-serif;
}

#content-promotion > .info-promotion p > strong {
  font-size: 2.1rem;
  font-family: inherit;
}

#content-promotion > .info-promotion a {
  font-size: 1.6rem;
  font-family: "Inter", sans-serif;
  font-weight: 800;
  color: #0071eb;
  display: flex;
  align-items: center;
  margin-left: 8px;
  text-decoration: none;
}

@media screen and (max-width: 480px) {
  #content-promotion {
    display: none;
  }
}
</style>
