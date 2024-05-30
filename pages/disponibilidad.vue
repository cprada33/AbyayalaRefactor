<template>
  <BookingRoomOptions />
</template>

<script>
import cabanas from '../assets/cabanas.json';
export default {
  data() {
    return {
      rooms: cabanas.filter((item) => item.pick === true),
    };
  },
};
</script>
