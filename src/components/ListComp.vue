<template>
  <div>
    <h1>list start</h1>
    <ul>
      <li v-for="item in items" :key="item.id">{{ item.message }}</li>
    </ul>
    <h1>list end</h1>
  </div>
</template>

<script>
export default {
  props: {
    items: Array
  }
};
</script>

<style scoped>
.app-thing {
  color: green;
}
</style>
