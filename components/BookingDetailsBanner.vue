<template>
  <v-container :fluid="true" class="pa-0 h-100 py-3 pr-15">
    <v-row class="h-100">
      <v-col cols="12" class="bg-grey h-100 rounded-lg px-7">
        <div class="py-3">
          <span class="texto-main" style="font-weight: 900"
            >DETALLES DE RESERVA</span
          >
        </div>
        <v-divider :thickness="4" class="border-opacity-50" />
        <div class="py-4">
          <div class="d-flex justify-space-between">
            <span class="texto-main" style="font-weight: 700"
              >TIPO DE CABAÑA
            </span>
            <span class="texto-main" style="font-weight: 400">SAFARI</span>
          </div>
          <div class="d-flex justify-space-between">
            <span class="texto-main" style="font-weight: 700"
              >CANTIDAD DE CABAÑAS </span
            ><span class="texto-main" style="font-weight: 400">3</span>
          </div>
          <div class="d-flex justify-space-between">
            <span class="texto-main" style="font-weight: 700"
              >FECHA DE ENTRADA </span
            ><span class="texto-main" style="font-weight: 400">20/07/2024</span>
          </div>
          <div class="d-flex justify-space-between pb-3">
            <span class="texto-main" style="font-weight: 700"
              >FECHA DE SALIDA </span
            ><span class="texto-main" style="font-weight: 400">23/07/2024</span>
          </div>
          <v-divider :thickness="4" class="border-opacity-50" />
          <div class="d-flex align-center pt-3">
            <v-col cols="6" class="text-start">
              <span> ¿Tienes código de descuento? </span>
            </v-col>
            <v-col cols="6">
              <v-text-field label="Código" variant="solo" :hide-details="true">
              </v-text-field>
            </v-col>
          </div>
          <div class="d-flex justify-space-between pt-3">
            <span class="texto-main" style="font-weight: 700"
              >PRECIO TOTAL </span
            ><span class="texto-main" style="font-weight: 400">960.000</span>
          </div>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>
