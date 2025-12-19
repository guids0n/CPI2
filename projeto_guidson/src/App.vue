<script setup lang="ts">
import CalculadoraSoma from './components/CalculadoraSoma.vue'
</script>

<template>
  <div class="tela">
    <h1>Projeto por Guidson Barreto de Jesus Silva</h1>
    <CalculadoraSoma />
  </div>
</template>

<style>
body {
  margin: 0;
  background-color: #8be0b6;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.tela {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
}

h1 {
  color: #444;
  margin-bottom: 20px;
}
</style>
