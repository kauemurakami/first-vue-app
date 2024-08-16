<script setup>
import { reactive, ref } from 'vue'

const counter = reactive({ count: 0 })

function incremment() {
  counter.count++
}

function decrement() {
  counter.count--
}

</script>

<template>
  
    <div class="container">
      <h1 class="centeredTitle">Count is: {{ counter.count }}</h1>
    </div> 
    <br/>
    <button type="button" class="btn btn-outline-primary btn-sm btn-mr" v-on:click="incremment"> + </button>
    <button type="button" class="btn btn-outline-danger btn-sm" v-on:click="decrement"> - </button>
</template>

<style>
.btn-mr {
  margin-right: 10px;
}
.container {
  display: flex;
  justify-content: center; /* Centraliza horizontalmente */
  align-items: center; /* Centraliza verticalmente */
  /* Define a altura do contêiner, pode ser ajustado conforme necessário */
}

.centeredTitle {
  text-align: center; /* Opcional, centraliza o texto dentro do elemento */
}
</style>

