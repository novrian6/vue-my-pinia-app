<template>
  <div class="app">
    <h1>Pinia Counter App</h1>
    <p>Count: {{ counter.count }}</p>
    <button @click="counter.increment">+</button>
    <button @click="counter.decrement">-</button>
  </div>
</template>

<script setup>
import { useCounterStore } from './stores/counter'
const counter = useCounterStore()
</script>

<style>
.app {
  text-align: center;
  font-family: sans-serif;
  padding: 2rem;
}
button {
  margin: 0.5rem;
  padding: 0.5rem 1rem;
}
</style>