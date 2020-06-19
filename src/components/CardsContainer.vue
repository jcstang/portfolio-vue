<template>
  <div class="container columns">
    <Card v-for="item in items" :key="item.id" msg="hi" />
  </div>
</template>

<script>
import Card from "./Card";

export default {
  components: {
    Card
  },
  props: {
    items: Array
  }
};
</script>

<style scoped>
.container {
  border: 1px dotted green;
}
</style>