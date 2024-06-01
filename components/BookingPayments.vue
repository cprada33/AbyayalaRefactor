<template>
  <v-container>
    <v-row>
      <v-col cols="12" class="text-center">
        <span class="texto-title color-main">METODOS DE PAGO</span>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" class="d-flex flex-column ga-2">
        <div>Transferencia bancaria</div>
        <div>
          <v-file-input
            label="Comprobante de pago"
            variant="outlined"
            prepend-inner-icon="mdi-paperclip"
            :prepend-icon="false"
          ></v-file-input>
        </div>
        <div class="text-center">
          <v-btn to="confirmacion" class="bg-second color-white"
            >RESERVAR</v-btn
          >
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>
