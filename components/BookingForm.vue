<template>
  <v-container :fluid="true">
    <v-row>
      <v-col cols="9" class="text-center">
        <v-row>
          <v-col cols="12">
            <span>DATOS DE RESERVA</span>
          </v-col>
        </v-row>
        <v-row>
          <v-col>
            <v-form>
              <v-container :fluid="true">
                <v-row>
                  <v-col cols="6">
                    <v-text-field label="Nombre completo"> </v-text-field>
                  </v-col>
                  <v-col cols="6">
                    <v-text-field label="Número de celular"> </v-text-field>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col cols="6">
                    <v-text-field label="Correo electronico"> </v-text-field>
                  </v-col>
                  <v-col cols="6">
                    <v-text-field label="Número de cédula"> </v-text-field>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col cols="3">
                    <v-text-field label="Número de cédula"> </v-text-field>
                  </v-col>
                  <v-col cols="3">
                    <v-text-field label="Acompañantes"> </v-text-field>
                  </v-col>
                  <v-col cols="6">
                    <v-text-field label="Nombres y cédulas de los acompañantes">
                    </v-text-field>
                  </v-col>
                </v-row>
                <v-row>
                  <v-col>
                    <v-btn to="confirmacion">PAGAR</v-btn>
                  </v-col>
                </v-row>
              </v-container>
            </v-form>
          </v-col>
        </v-row>
      </v-col>

      <v-col cols="3" class="bg-grey">
        <div>
          <span>DETALLES DE RESERVA</span>
        </div>
        <div>
          <div>
            <span>TIPO DE CABAÑA: <span>SAFARI</span></span>
          </div>
          <div>
            <span>TIPO DE CABAÑA: <span>SAFARI</span></span>
          </div>
          <div>
            <span>TIPO DE CABAÑA: <span>SAFARI</span></span>
          </div>
          <div>
            <span>TIPO DE CABAÑA: <span>SAFARI</span></span>
          </div>
          <div>
            <span>TIPO DE CABAÑA: <span>SAFARI</span></span>
          </div>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>
