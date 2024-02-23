<script>
export default {
data() {
  return {
    contador: 0
  }
},
methods: {
  incrementar() {
    this.contador++;
  },
  decrementar() {
    if (this.contador > 0) this.contador--;
  },
  reiniciar() {
    this.contador = 0
  }
}
}

</script>

<template>
  <button @click="incrementar">+</button>
  <button @click="decrementar">-</button>
  <button @click="reiniciar">0</button>
  <p>valor do contador: {{ contador }}</p>
</template>

<style scoped>
button {
  color: blueviolet;
  font-weight: bold;
  background-color: black;
  border: none;
}
</style>