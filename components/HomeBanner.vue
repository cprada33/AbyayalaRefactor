<template>
  <v-container :fluid="true" class="pa-0 pb-5">
    <v-row>
      <v-col cols="4">
        <img
          src="https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fbannermujer.png?alt=media&token=cfda4ded-25e4-4c97-9065-ca6f497e344c"
          alt="banner"
          style="width: 110%; height: 100%; object-fit: contain"
        />
      </v-col>
      <v-col cols="8" class="d-flex flex-column">
        <v-row class="mt-15">
          <v-col
            class="d-flex justify-center mx-5"
            style="
              font-size: 7rem;
              font-weight: 900;
              color: #00bbd6;
              height: 150px;
            "
            >BIENVENIDOS</v-col
          >
        </v-row>
        <v-row>
          <v-col
            class="d-flex justify-center align-center mx-10"
            style="
              font-size: 7rem;
              font-weight: 900;
              color: #228fa2;
              height: 150px;
            "
            >A</v-col
          >
        </v-row>
        <v-row class="mt-n10">
          <v-col
            class="d-flex justify-center mx-10"
            style="
              font-size: 7rem;
              font-weight: 900;
              color: #228fa2;
              height: 150px;
            "
          >
            <span>LA MONTAÑA</span>
          </v-col>
        </v-row>
        <v-row class="mb-15">
          <v-col
            class="d-flex justify-center align-center mx-10"
            style="font-size: 1.3rem; text-align: center"
            >Bienvenidos a esta montaña donde se rinde tributo a la herencia y
            legado ancestral, bienvenidos a nuestra casa.</v-col
          >
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script lang="ts" setup>
const dateValue = ref();
</script>
