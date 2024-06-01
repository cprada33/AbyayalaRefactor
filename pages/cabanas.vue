<template>
  <div class="bg-main text-center py-3">
    <div class="py-3">
      <span style="font-weight: 900; font-size: 2.5rem; color: white"
        >CABAÑAS SAFARI</span
      >
    </div>
    <GeneralImagesBanner :styling="stylingCabanas" :content="content" />
  </div>
  <v-container :fluid="true" class="pa-0 pb-7 px-15">
    <v-row class="pt-7">
      <v-col class="text-center">
        <span class="texto-title color-main">CABAÑA ANCESTRAL</span>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="6" style="max-height: 450px">
        <div style="max-height: 450px">
          <img
            src="/assets/imgs/cabanas/ancestral.jpeg"
            alt="Cabaña Ancestral"
            style="width: 100%; max-height: 450px; object-fit: cover"
          />
        </div>
      </v-col>
      <v-col cols="6" class="d-flex flex-column text-center justify-center">
        <span class="color-third texto-subtitle">AWÁ KWAIKER</span>
        <span class="texto-main"
          >Pueblo Indio Americano, que en lengua Awapit significa "Gente de la
          montaña".</span
        >
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import cabanas from '../assets/cabanas.json';

export default {
  data() {
    return {
      stylingCabanas: {
        divStyle: 'height: 100%',
        imgStyle: 'height: 100%; width: 87%; object-fit: cover;',
      },
      content: cabanas.filter((item) => item.tipo === 'Safari'),
    };
  },
};
</script>
