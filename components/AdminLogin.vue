<template>
  <v-container :fluid="true" class="w-50 bg-third">
    <v-row>
      <v-cols cols="12">
        <img
          src="../assets/imgs/logoMain.png"
          alt="Logo Abya Yala"
          style="max-width: 40%"
        />
      </v-cols>
    </v-row>
    <v-row class="d-flex flex-column">
      <v-col class="d-flex flex-column">
        <span>INGRESA TUS CREDENCIALES</span>
        <span>Si tienes una cuenta de administración, ingresa tus datos:</span>
        <v-text-field label="Correo electronico"></v-text-field>
        <v-text-field label="Contraseña"></v-text-field>
        <v-btn>INGRESAR</v-btn>
        <v-btn>REGISTRAS NUEVO ADMIN</v-btn>
      </v-col>
      <v-row>
        <v-col>
          <span>¿No puedes ingresar? Contacta con <span>Dread Blue</span></span>
        </v-col>
      </v-row>
    </v-row>
    <v-row> </v-row>
  </v-container>
</template>
