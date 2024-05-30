<template>
  <v-container :fluid="true">
    <v-row class="px-1">
      <v-col cols="3" v-for="item in content" :style="styling.divStyle">
        <v-row class="d-flex flex-column" style="height: 100%">
          <v-col class="text-center" style="height: 100%">
            <img
              :src="item.src"
              alt="imagen"
              style="height: 100%; width: 100%; object-fit: cover"
              :class="styling.imgClass"
            />
          </v-col>
          <v-col
            v-if="item.nombre"
            class="text-center pa-0"
            style="font-weight: 700; font-size: 1.1rem; color: white"
          >
            {{ item.nombre }}
          </v-col>
          <v-col
            v-if="item.descripcion"
            class="d-flex text-center pa-0 justify-center"
            style="
              font-weight: 400;
              font-size: 1.1rem;
              color: black;
              width: 87%;
            "
          >
            {{ item.descripcion }}
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  props: {
    styling: Object,
    content: Object,
  },
  setup() {
    const thisRoute = useRoute().path;
    return {
      thisRoute,
    };
  },
  mounted() {
    console.log(this.thisRoute);
  },
};
</script>
