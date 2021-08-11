<template>
  <div class="cryptogradient">
    <nuxt/>
  </div>
</template>

<script>
export default {
  head() {
    return {
      bodyAttrs: {
        class: 'cryptopage'
      }
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Russo+One&family=Source+Sans+Pro:wght@400;900&display=swap');

.cryptopage {
  color: #fff;
  font-family: 'Source Sans Pro', sans-serif;
  height: 100vh;
  background: rgb(5,9,27);
  background: linear-gradient(90deg, rgba(5,9,27,1) 0%, rgba(9,9,121,1) 47%, rgba(16,31,93,1) 100%);
}
.cryptogradient {
  background: url("/earth-dotted.png") bottom right no-repeat;
  background-size: 500px;
  height: 100vh;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}
</style>
