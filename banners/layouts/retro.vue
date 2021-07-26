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
.retropage {
  background: url("/pixel_effect.png") top center repeat-x #1d1725;
  color: #fff;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}
</style>
