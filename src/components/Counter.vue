<template>
  <div class="first">
    <h2>Counter ref: {{ count }}</h2>
    <button @click="incrementRef">increment</button>
    <button @click="decrementRef">decrement</button>
  </div>
  <div class="two">
    <h2>Conter Reactive: {{ state.counter }}</h2>
    <button @click="incrementReactive">incrementReactive</button>
    <button @click="decrementReactive">decrementReactive</button>
  </div>
</template>
<script setup>
import { ref, reactive } from 'vue';
//belajar menggunakan ref
const count = ref(0); //reactive single value
const incrementRef = () => count.value++;
const decrementRef = () => count.value--;

//belajr menggunakan reactive
const state = reactive({ counter: 0 }); //reactuve object
const incrementReactive = () => state.counter++;
const decrementReactive = () => state.counter--;
</script>
<style lang=""></style>
