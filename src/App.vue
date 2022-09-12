<template>

  <div>
    <button @click="decrement">-</button>
    {{number}}

    <button @click="increment">+</button>
  </div>
  
</template>

<script>
import {ref } from 'vue';
import useCounter from './helpers/count';

export default {
  setup(){

    const number = ref(0)

    const {increment, decrement} = useCounter(number)
    return{increment, number, decrement}
  }

}
</script>

<style>

</style>