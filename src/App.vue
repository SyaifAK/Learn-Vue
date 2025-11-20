<script setup>
const name = 'Syaif';
const year = 2025;
</script>

<template>
  <main>
    <h1>Halo, {{ name }}</h1>
    <p>Learn Vue in {{ year }}</p>
  </main>

  <footer>
    <p>© {{ name }} {{ year }}</p>
  </footer>
</template>

<style scoped>
main {
  font-size: 50px;
  text-align: center;
}

footer {
  text-align: center;
  height: 50px;
  background-color: green;
  color: white;
}
</style>
