<script>
export default {
  name: "ThePromotionWindow",
  data() {
      return {
          showWindow: true
      }
  }
};
</script>

<template>
  <div id="window-container" v-if="showWindow">
    <div class="close-window" @click="showWindow = false">
      <svg
        width="16"
        height="16"
        viewBox="0 0 16 16"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
        class="ads-corner-banner-close-icon-desktop"
        aria-hidden="true"
      >
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M1.47021 2.53075L6.93989 8.00042L1.47021 13.4701L2.53087 14.5308L8.00054 9.06108L13.4702 14.5308L14.5309 13.4701L9.06121 8.00042L14.5309 2.53075L13.4702 1.47009L8.00054 6.93976L2.53087 1.47009L1.47021 2.53075Z"
          fill="#000"
        ></path>
      </svg>
    </div>

    <div id="content-promotion">
        <div class="info-promotion">
            <h2>
                Planos para todos os bolsos.
                A partir de R$18,90.
            </h2>
            
            <button id="btn-window">Conhecer planos</button>
        </div>
    </div>

    <img src="../assets/pipoca-icon.png" alt="Icon" width="100">
  </div>
</template>

<style>
    #window-container {
        display: flex;
        align-items: center;
        height: 15.4rem;
        max-width: 50rem;
        position: relative;
        right: 3rem;
        bottom: 3rem;
        position: fixed;
        padding: 2.4rem;
        background: #fff;
        border-radius: 1rem;
    }

    #window-container .close-window {
        position: absolute;
        right: 1rem;
        top: 1rem;
        cursor: pointer;
    }

    #window-container #content-promotion {
        width: 100%;
        display: flex;
        justify-content: space-between;
    }

    #window-container #content-promotion > .info-promotion {
        display: flex;
        flex-direction: column;
        gap: 2rem;
    }

    #window-container #content-promotion > .info-promotion h2 {
        font-size: 2rem;
        font-family: 'Inter', sans-serif;
        color: #333333;
    }

    #window-container #content-promotion > .info-promotion button#btn-window {
        background: #4969E4;
        border-radius: 5px;
        border: none;
        font-size: 1.6rem;
        font-family: 'Inter', sans-serif;
        font-weight: 500;
        color: #fff;
        padding: .8rem 2rem;
        width: 80%;
        cursor: pointer;
    }

    @media screen and (max-width: 550px) {
      #window-container {
        width: 90%;
      }

      #window-container img {
        width: 7rem;
      }
    }

    @media screen and (max-width: 400px) {
      #window-container img {
        display: none;
      }
    }
</style>