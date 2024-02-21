<script setup>
  import { ref } from "vue";

  const contador = ref(0)

  function decrementar() {
    contador.value--
  }
</script>

<template>
  <button @click="contador++" >+</button>
  <button @click="decrementar">-</button>
  <p>Valor do Contador: {{ contador }}</p>
</template>

<style scoped></style>
