<template>
  <nav class="navbar is-dark" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <img :src="url" class="App-logo" alt="logo" />
      <h1>Jacob Stanger</h1>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Nav',
  props: {
    url: String,
  },
};
</script>

<style scoped>
.App-logo {
  width: 3vw;
  height: auto;
}
</style>
