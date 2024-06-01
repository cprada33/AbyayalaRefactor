<template>
  <HomeBanner />
  <HomeRooms />
  <GeneralImagesBanner :styling="styling" :content="content" />
  <HomeLocation />
</template>

<script>
export default {
  data() {
    return {
      styling: {
        divStyle: 'max-height: 250px',
        imgClass: 'rounded-xl',
      },
      content: {
        imagen1: {
          src: 'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        },
        imagen2: {
          src: 'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        },
        imagen3: {
          src: 'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        },
        imagen4: {
          src: 'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        },
        imagen5: {
          src: 'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        },
        imagen6: {
          src: 'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        },
        imagen7: {
          src: 'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        },
        imagen8: {
          src: 'https://firebasestorage.googleapis.com/v0/b/abyayala-c7fa8.appspot.com/o/assets%2Fancestral.jpeg?alt=media&token=d3bf286c-baa8-4702-adec-0dfc710cd297',
        },
      },
    };
  },
};
</script>
