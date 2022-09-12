<template>

  <div>

    Halo nama saya adalah {{name}}
  </div>
  
</template>

<script>
import {ref } from 'vue';

export default {
  setup(){
    const name = ref("Jazuli")
  
    setTimeout( () => {
    
      name.value = "Muhammad"

    }, 2000)
    return {
      name
    }
  }

}
</script>

<style>

</style>