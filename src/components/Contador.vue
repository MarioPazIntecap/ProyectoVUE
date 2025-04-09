<template>
<h1>Ejemplo de Reactividad</h1>
<p>{{ contador }}</p>
<button @click="incrementar">Incrementar</button>
<button @click="decrementar">Decrementar</button>
</template>

<script setup>
import {ref} from 'vue';
const contador = ref(1);

const incrementar = () =>{
  contador.value++;


}

const decrementar = () =>{
  contador.value--;
}

</script>

<style scoped>
p {
  color: red;
  text-align: center;
}

h1 {
  color: green;
  text-align: center;
}
</style>