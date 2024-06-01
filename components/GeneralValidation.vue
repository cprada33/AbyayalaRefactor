<template>
  <div>
    <v-img
      class="mx-auto my-6"
      max-width="228"
      src="/assets/imgs/logoMain.png"
    ></v-img>
    <v-card
      class="mx-auto pa-12 pb-8"
      elevation="8"
      max-width="448"
      rounded="lg"
    >
      <div class="text-subtitle-1 text-medium-emphasis font-raleway">
        {{ formato.InputUno[0] }}
      </div>

      <v-text-field
        density="compact"
        :placeholder="formato.InputUno[1]"
        :prepend-inner-icon="formato.InputUno[2]"
        variant="outlined"
      ></v-text-field>

      <div
        class="text-subtitle-1 text-medium-emphasis d-flex align-center justify-space-between font-raleway"
      >
        {{ formato.InputDos[0] }}

        <a
          v-if="formato.Login"
          class="text-caption text-decoration-none text-blue font-raleway"
          href="#"
          rel="noopener noreferrer"
          target="_blank"
        >
          ¿Olvidaste tu contraseña?</a
        >
      </div>

      <v-text-field
        v-if="formato.contrasena"
        :append-inner-icon="visible ? 'mdi-eye-off' : 'mdi-eye'"
        :type="visible ? 'text' : 'password'"
        density="compact"
        :placeholder="formato.InputDos[1]"
        :prepend-inner-icon="formato.InputDos[2]"
        variant="outlined"
        @click:append-inner="visible = !visible"
      ></v-text-field>

      <v-text-field
        v-if="!formato.contrasena"
        density="compact"
        :placeholder="formato.InputDos[1]"
        :prepend-inner-icon="formato.InputDos[2]"
        variant="outlined"
      ></v-text-field>

      <v-card class="mb-12" color="surface-variant" variant="tonal">
        <v-card-text class="text-medium-emphasis text-caption font-raleway">
          {{ formato.Descripcion }}
        </v-card-text>
      </v-card>

      <v-btn
        class="mb-8 font-raleway"
        color="blue"
        size="large"
        variant="tonal"
        block
        :to="formato.btn[1]"
      >
        {{ formato.btn[0] }}
      </v-btn>
    </v-card>
  </div>
</template>

<script>
export default {
  props: {
    formato: Object,
  },
  data: () => ({
    visible: false,
  }),
};
</script>
