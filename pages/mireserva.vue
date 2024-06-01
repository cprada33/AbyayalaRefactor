<template>
  <GeneralValidation :formato="info" />
</template>

<script>
export default {
  data() {
    return {
      info: {
        InputUno: ['Codigo de reserva', 'Codigo', 'mdi-ticket'],
        InputDos: [
          'Correo titular',
          'Ingresa tu correo electronico',
          'mdi-email-outline',
        ],
        Descripcion:
          '¡Hola! Bienvenido a casa, desde aquí podrás enviar solicitudes para modificar tus fechas de reserva, el titular o realizar la reserva anticipada de tu menú de comidas durante tu estancia',
        Login: false,
        btn: ['Gestionar reserva', 'reserva'],
      },
    };
  },
};
</script>
