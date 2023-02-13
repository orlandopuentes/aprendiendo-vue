<script setup>
import { useCounterStore } from '@/store/counter.js'
import { storeToRefs } from 'pinia';

const useCounter = useCounterStore()
const { increment } = useCounter
const { double, count } = storeToRefs(useCounter)
</script>

<template>
  <h1>
    home counter: {{ count }}
  </h1>
  <h2>Doble: {{ double }}</h2>
  <button @click="increment">Increment</button>
</template>
