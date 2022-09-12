<template>

  <div>

    Ini adalah angka {{number}}
  </div>
  
</template>

<script>
import {ref } from 'vue';

export default {
  setup(){
    const number = ref(0)
  
    setInterval( () => {
    
      number.value++
    }, 500)
    return {
      number
    }
  }

}
</script>

<style>

</style>