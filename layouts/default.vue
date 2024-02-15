<template>
  <div class="leading-normal tracking-normal text-white gradient">
    <Header />
    <slot />
    <Footer/>
  </div>
</template>

<script lang="ts" setup>

</script>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
.gradient {
  background: linear-gradient(90deg, #BCBCBC 0%, #38B380 100%);
}
</style>