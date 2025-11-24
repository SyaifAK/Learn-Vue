<script setup>
const button = true;
const tes = 'cupu';
</script>
<template>
  <div>
    <h1>Ini halaman Halo Vuse {{ tes }}</h1>
    <p>bangke, {{ tes }}</p>
    <button :disabled="button">ini button</button>
  </div>
</template>
<style>
h1 {
  color: blue;
  background-color: gray;
}
</style>
