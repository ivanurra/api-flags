<template>
  <div class="container">
    <h2 class="text-center">COUNTRIES API</h2>
    <Continents />
    <CardList />
  </div>
</template>

<script>
import CardList from "./components/CardList.vue";
import Continents from './components/Continents.vue';
export default {
  name: "App",
  components: {
    CardList,
    Continents,
  },
};
</script>

<style>
.container{
  background: rgb(244, 244, 244);
}
</style>

