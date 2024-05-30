<template>
  <v-container>
    <v-row v-for="item in rooms">
      <v-col cols="6">
        <img :src="item.src" alt="Cabaña Safari" class="w-100" />
      </v-col>
      <v-col cols="6">
        <div>
          <span>{{ item.nombre }}</span>
        </div>
        <div class="d-flex flex-column">
          <div v-for="detalle in item.detalles">{{ detalle }}</div>
        </div>
        <div>
          <v-btn> - </v-btn>
          <span> 0 </span>
          <v-btn> + </v-btn>
        </div>
        <div>
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
