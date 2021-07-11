<template>
  <input 
  type="text"
  placeholder="Find a country"
  class="form-control my-3"
  v-model="texto"
  @keyup="procesarInput"
  >
</template>

<script>
import { ref } from '@vue/reactivity'
export default {
    setup(){
        const texto = ref('')

        const procesarInput = () => {
            console.log(texto.value)
        }

        return {texto, procesarInput}
    }
}
</script>
