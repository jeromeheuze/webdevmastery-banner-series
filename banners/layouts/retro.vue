<template>
  <div>
    <nuxt/>
  </div>
</template>

<script>
export default {
  head() {
    return {
      bodyAttrs: {
        class: 'retropage'
      }
    }
  }
}
</script>

<style>
@font-face {
  font-family: 'Kenney Future';
  src: url('https://storage.googleapis.com/tutorial_asset/fonts/Kenney-Future.woff2') format('woff2'),
  url('https://storage.googleapis.com/tutorial_asset/fonts/Kenney-Future.woff') format('woff');
  font-weight: normal;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Kenney Thick';
  src: url('https://storage.googleapis.com/tutorial_asset/fonts/Kenney-Thick.woff2') format('woff2'),
  url('https://storage.googleapis.com/tutorial_asset/fonts/Kenney-Thick.woff') format('woff');
  font-weight: normal;
  font-style: normal;
  font-display: swap;
}
.retropage {
  background: url("/pixel_effect.png") top center repeat-x #1d1725;
  color: #fff;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}
</style>
