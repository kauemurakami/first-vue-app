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
  
    <h1>Count is: {{ counter.count }}</h1>
    <br/>
    <button type="button" class="btn btn-outline-primary btn-sm" v-on:click="incremment"> + </button>
    <button type="button" class="btn btn-outline-danger btn-sm" v-on:click="decrement"> - </button>
</template>



