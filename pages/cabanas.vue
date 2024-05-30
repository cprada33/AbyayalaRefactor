<template>
  <div class="bg-main text-center py-3">
    <div class="py-3">
      <span style="font-weight: 900; font-size: 2.5rem; color: white"
        >CABAÑAS SAFARI</span
      >
    </div>
    <BannerImages :styling="stylingCabanas" :content="content" />
  </div>
</template>

<script>
import cabanas from '../assets/cabanas.json';

export default {
  data() {
    return {
      stylingCabanas: {
        divStyle: 'height: 100%',
        imgStyle: 'height: 100%; width: 87%; object-fit: cover;',
      },
      content: cabanas.filter((item) => item.tipo === 'Safari'),
    };
  },
};
</script>
