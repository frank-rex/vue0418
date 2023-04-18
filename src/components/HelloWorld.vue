<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  
  <p>
    IG
    <a href="https://www.instagram.com/_franxx.k/" target="_blank">_franxx.k</a>
    follow
  </p>
  <p class="read-the-docs"> </p>
</template>

<style scoped>
.read-the-docs {
  color: #ed0e0e;
}
</style>
