<script setup lang="ts">
import { ref, computed } from 'vue'

const numero1 = ref(0)
const numero2 = ref(0)

const resultado = computed(() => {
  return numero1.value + numero2.value
})
</script>

<template>
  <div class="calculadora">
    <h2>➕ Somadora Vue</h2>

    <div class="inputs">
      <input type="number" v-model.number="numero1" placeholder="0" />
      <span class="sinal">+</span>
      <input type="number" v-model.number="numero2" placeholder="0" />
    </div>

    <div class="resultado-box">
      <p>Resultado:</p>
      <strong class="valor">{{ resultado }}</strong>
    </div>
  </div>
</template>

<style scoped>
.calculadora {
  background-color: #f8f9fa;
  border: 2px solid #074d38;
  border-radius: 12px;
  padding: 30px;
  max-width: 350px;
  margin: 0 auto;
  text-align: center;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  color: #333;
}

.inputs {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  margin-bottom: 20px;
}

input {
  width: 80px;
  padding: 10px;
  font-size: 18px;
  text-align: center;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.sinal {
  font-weight: bold;
  font-size: 24px;
  color: #2c8f39;
}

.resultado-box {
  background-color: #16d39a;
  color: white;
  padding: 15px;
  border-radius: 8px;
}

.valor {
  font-size: 32px;
  display: block;
}
</style>
