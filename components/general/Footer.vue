<template>
  <v-container
    :fluid="true"
    class="pa-0 mt-10"
    style="color: white; font-size: 0.9rem"
  >
    <v-row class="bg-main">
      <v-col
        cols="3"
        class="d-flex flex-column text-center justify-center"
        style="font-style: italic"
      >
        <NuxtLink>
          <img
            src="../../assets/imgs/logo.svg"
            alt="Logo"
            style="max-width: 80%"
            class="pb-3"
          />
        </NuxtLink>
        <span>Nimaima, Cundinamarca</span>
        <span>reservas.abyayalahostel@gmail.com</span>
      </v-col>
      <v-col
        cols="6"
        class="d-flex flex-column justify-center text-center align-end"
      >
        <div class="w-25">SIGUENOS</div>
        <div class="d-flex w-25 ga-2 justify-center">
          <v-icon icon="mdi-facebook"></v-icon>
          <v-icon icon="mdi-instagram"></v-icon>
          <v-icon icon="mdi-whatsapp"></v-icon>
        </div>
      </v-col>
      <v-col cols="3">
        <NuxtLink>ABYA YALA HOSTEL</NuxtLink>
        <NuxtLink></NuxtLink>
      </v-col>
    </v-row>
    <v-row class="bg-second">
      <v-col cols="6" class="d-flex ga-5 pl-15">
        <NuxtLink>Términos y condiciones</NuxtLink>
        <NuxtLink>Maps</NuxtLink>
      </v-col>
      <v-col cols="6" class="justify-end">
        <div class="text-end pr-10">
          All rights reserved - Desarrollado por
          <a href="www.dreadblue.com">Dread Blue SAS</a>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>
