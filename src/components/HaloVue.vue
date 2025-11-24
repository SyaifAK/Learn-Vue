<script setup>
import { ref } from 'vue';

const button = true;
const tes = 'cupu';
const a = ref(0);
//user
const role = ref('user');
</script>
<template>
  <div>
    <h1>Ini halaman Halo Vuse {{ tes }}</h1>
    <p>bangke, {{ tes }}</p>
    <button :disabled="button">ini button</button>
    <br />
    <h2>{{ a }}</h2>
    <button @click="a++">sentuh aku</button>
  </div>

  <div class="condition">
    <h2>Tekan tombol dibawah ini</h2>
    <button @click="role = 'admin'">admin</button>
    <button @click="role = 'user'">user</button>

    <p v-if="role === 'admin'">Selamat datang admin wkwkwk</p>
    <p v-else-if="role === 'user'">Selanat daataaang user elek</p>
    <p v-else>anomali bjr ?</p>
  </div>
</template>
<style>
h1 {
  color: blue;
  background-color: gray;
}

.condition {
  padding-top: 30px;
}
</style>
