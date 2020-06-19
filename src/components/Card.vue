<template>
  <div class="container column card">
    <i :class="item.fontAwesomeIcon"></i>
    <p>hello {{msg}}</p>
  </div>
</template>

<script>
export default {
  props: {
    item: Object,
    msg: String
  }
};
</script>

<style scoped>
</style>