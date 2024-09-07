<template>
  <div>
    <h1 class="h1">Mi primer componente</h1>

    <section>
      <h3>Número = {{ numero }}</h3>
    </section>

    <button class="btn" @click="aumentar">+1</button>
    🥸
    <button class="btn" @click="disminuir">-1</button>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'

// Definir una variable reactiva 'numero'
const numero = ref<number>(0)

// Función para aumentar el número
const aumentar = () => {
  numero.value++
}

// Función para disminuir el número
const disminuir = () => {
  numero.value--
}
</script>

<hr />
