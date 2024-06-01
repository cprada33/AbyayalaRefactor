<template>
  <div class="d-flex mx-13">
    <div class="d-flex align-center d-lg-none">
      <v-app-bar-nav-icon
        variant="text"
        @click.stop="drawer = !drawer"
      ></v-app-bar-nav-icon>
      <v-spacer></v-spacer>

      <v-navigation-drawer
        v-model="drawer"
        :location="$vuetify.display.mobile ? 'bottom' : undefined"
        temporary
      >
        <v-list-item
          v-for="route in routes"
          :to="route.route"
          :active="false"
          :title="route.name"
          style="font-size: 4rem"
        ></v-list-item>
      </v-navigation-drawer>
    </div>
    <div class="v-col-3">
      <NuxtLink to="/">
        <img
          src="../../assets/imgs/logoMain.png"
          alt="logo"
          style="width: 90%"
        />
      </NuxtLink>
    </div>
    <div class="d-flex v-col-auto justify-space-evenly v-col-9 pa-0">
      <v-list-item
        v-for="route in routes"
        :to="route.route"
        :title="route.name"
        :active="false"
      ></v-list-item>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    drawer: false,
    group: null,
    routes: [
      {
        name: 'Inicio',
        route: '/',
      },
      {
        name: 'Actividades',
        route: '/actividades',
      },
      {
        name: 'Cabañas',
        route: '/cabanas',
      },
      {
        name: '¿Quienes somos?',
        route: '/quienes-somos',
      },
      {
        name: 'Contacto',
        route: '/contacto',
      },
      {
        name: 'Mi reserva',
        route: '/mireserva',
      },
    ],
  }),

  watch: {
    group() {
      this.drawer = false;
    },
  },
};
</script>
