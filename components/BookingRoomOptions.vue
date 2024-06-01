<template>
  <v-container
    class="d-flex flex-column ga-15 texto-main pa-0 px-15 py-7"
    :fluid="true"
  >
    <v-row v-for="item in rooms" :class="`elevation-${5}`">
      <v-col cols="6" style="height: 450px">
        <img
          :src="item.src"
          alt="Cabaña Safari"
          class="w-100"
          style="max-height: 100%; object-fit: cover"
        />
      </v-col>
      <v-col cols="6">
        <div class="text-center">
          <span class="texto-title color-second">
            CABAÑA <span>{{ item.tipo.toUpperCase() }}</span></span
          >
        </div>
        <div class="d-flex flex-column align-center ga-3">
          <div v-for="detalle in item.detalles">{{ detalle }}</div>
        </div>
        <div class="text-center py-5">
          <v-btn> - </v-btn>
          <span> 0 </span>
          <v-btn> + </v-btn>
        </div>
        <div class="text-center">
          <v-btn to="reservar">RESERVAR</v-btn>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import cabanas from '../assets/cabanas.json';
export default {
  data() {
    return {
      rooms: cabanas.filter((item) => item.pick === true),
    };
  },
};
</script>
