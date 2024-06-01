<template>
  <GeneralValidation :formato="info" />
</template>

<script>
export default {
  data() {
    return {
      info: {
        InputUno: ['Cuenta', 'Correo electronico', 'mdi-email-outline'],
        InputDos: ['Contraseña', 'Ingresa tu contraseña', 'mdi-lock-outline'],
        Descripcion:
          'Warning: After 3 consecutive failed login attempts, you account will be temporarily locked for three hours. If you must login now, you can also click "Forgot login password?" below to reset the login password.',
        Login: true,
        btn: ['Ingresar', '/admin'],
        contrasena: true,
      },
    };
  },
};
</script>
