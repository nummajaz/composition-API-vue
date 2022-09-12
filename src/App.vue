<template>

  <div>

    Halo nama saya adalah {{state.user.name}} <br>
    status saya adalah {{state.loading}}

  </div>
  
</template>

<script>
import {reactive} from 'vue';

export default {
  setup(){
    const state = reactive({
      loading : false,
      user: {
        name: "jazuli",
        umur: 25
      },
      info:{
        status : "wiraswasta",
        hobi: "turu"
      }

    })
    setTimeout(() =>{
      state.user.name  = "Nur Muhammad Jazuli",
      state.loading = true
    }, 2000)
    
    return{
      state
    }
  }

}
</script>

<style>

</style>