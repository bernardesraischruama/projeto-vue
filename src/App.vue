<script setup>
  import { ref } from "vue";

  const contador = ref(0)

  function incrementar() {
    contador.value++;
  }

  function decrementar() {
    if (contador.value > 0) contador.value--
  }

  function recomeçar() {
    contador.value = 0
  }
</script>

<template>
  <div>
  <button @click="incrementar" >+</button>
  <button @click="decrementar">-</button>
  <button @click="recomeçar">recomeçar</button>
  <p>Valor do Contador: {{ contador }}</p>
  </div>
</template>

<style scoped>

</style>
