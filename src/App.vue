<script setup>
import { ref } from 'vue';
import Counter from './components/Counter.vue';
const name = 'Syaif';
const year = 2025;
const httml = '<h1>Halo Vue</h1>';
const image = ref('/che.png');

//fungsi ganti gambar
function changeImage() {
  image.value = image.value === '/che.png' ? '/kom.jpg' : '/che.png';
}
</script>

<template>
  <main>
    <div class="first">
      <h1>Halo, {{ name }}</h1>
      <p>Learn Vue in {{ year }}</p>
      <p v-html="httml"></p>
      <img :src="image" width="200" alt="" />
      <button @click="changeImage">Ganti gambar</button>
    </div>
    <div class="counter">
      <counter />
    </div>
  </main>

  <footer>
    <p>© {{ name }} {{ year }}</p>
  </footer>
</template>

<style scoped>
main {
  text-align: center;
}

.first {
  background-color: antiquewhite;
}
.counter {
  background-color: aqua;
}

footer {
  text-align: center;
  height: 50px;
  background-color: green;
  color: white;
}
</style>
