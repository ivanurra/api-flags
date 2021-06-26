<template>
  <div class="container">
    <h2 class="text-center">COUNTRIES API</h2>
    <CardList />
  </div>
</template>

<script>
import CardList from "./components/CardList.vue";
export default {
  name: "App",
  components: {
    CardList,
  },
};
</script>

