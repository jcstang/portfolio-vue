<template>
  <div class="container columns">
    <p>card container</p>
    <div class="column" v-for="item in items" :key="item.id">{{item.message}}</div>
    <Card />
  </div>
</template>

<script>
import Card from "./Card";

export default {
  components: {
    Card
  }
};
</script>

<style scoped>
.container {
  border: 1px dotted green;
}
</style>