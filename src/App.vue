<script setup>
import { ref } from 'vue'

const msg = ref('Enter text to create barcode');
  document.onkeypress = () =>{document.querySelector('h1').classList.add("encode")}
</script>

<template>
  <input v-model="msg">
  <br>
  <center><h1>{{ msg }}</h1></center>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Libre+Barcode+39&display=swap');
h1.encode{
   font-family: 'Libre Barcode 39';
   font-size:100px;
}
</style>