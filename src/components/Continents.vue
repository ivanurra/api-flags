<template>
<div 
class="text-center" 
style="margin-bottom: 40px;"
>
  <h3 class="text-center">Filter by Continent</h3>
  <div 
  class="btn-group" 
  role="group" 
  aria-label="Basic example">
    <button type="button" class="btn btn-dark" @click="filtro('Americas')">AM</button>
    <button type="button" class="btn btn-dark" @click="filtro('Europe')">EU</button>
    <button type="button" class="btn btn-dark" @click="filtro('Asia')">AS</button>
    <button type="button" class="btn btn-dark" @click="filtro('Oceania')">OC</button>
    <button type="button" class="btn btn-dark" @click="filtro('Africa')">AF</button>
    <button type="button" class="btn btn-dark" @click="filtro('')">ALL</button>
  </div>
</div>
</template>

<script>
import { useStore } from 'vuex';
export default {
  setup() {
    const store = useStore()

    const filtro = (region) => {
      store.dispatch('filtrarRegion', region)
    }

    return {filtro}
  }
};
</script>
