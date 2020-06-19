<template>
  <div class="container-fluid columns">
    <Card v-for="item in items" :key="item.id" :msg="item.message" :item="item" />
  </div>
</template>

<script>
import Card from "./Card";

export default {
  components: {
    Card
  },
  props: {
    items: Array,
    item: Object
  }
};
</script>

<style scoped>
.columns {
  margin: 1vw 2.5vw;
}
</style>