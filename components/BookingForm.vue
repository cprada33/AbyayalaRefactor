<template>
  <v-container :fluid="true">
    <v-row>
      <v-col cols="12" class="text-center">
        <v-row>
          <v-col cols="12">
            <span class="color-main texto-title">DATOS DE RESERVA</span>
          </v-col>
        </v-row>
        <v-row>
          <v-col>
            <v-form>
              <v-container :fluid="true">
                <v-row>
                  <v-col cols="6">
                    <v-text-field label="Nombre completo" variant="solo">
                    </v-text-field>
                  </v-col>
                  <v-col cols="6">
                    <v-text-field label="Número de celular" variant="solo">
                    </v-text-field>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col cols="6">
                    <v-text-field label="Correo electronico" variant="solo">
                    </v-text-field>
                  </v-col>
                  <v-col cols="6">
                    <v-text-field label="Número de cédula" variant="solo">
                    </v-text-field>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col cols="3">
                    <v-text-field label="Número de cédula" variant="solo">
                    </v-text-field>
                  </v-col>
                  <v-col cols="3">
                    <v-text-field label="Acompañantes" variant="solo" value="0">
                    </v-text-field>
                  </v-col>
                  <v-col cols="6">
                    <v-text-field
                      label="Nombres y cédulas de los acompañantes"
                      variant="solo"
                    >
                    </v-text-field>
                  </v-col>
                </v-row>
              </v-container>
            </v-form>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>
