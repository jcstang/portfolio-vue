<template>
  <div class="container-fluid">
    <nav class="navbar is-dark" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <img :src="url" class="App-logo" alt="logo" />
      </div>
      <div id="navbarBasicExample" class="navbar-menu">
        <div class="navbar-start">
          <a class="navbar-item" href="/">
            <p class="is-2">Jacob Stanger</p>
          </a>
        </div>
      </div>
    </nav>
  </div>
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
  margin: 0.77rem;
}
.container-fluid {
  padding: 0px;
}
nav {
  box-shadow: 2px 2px 30px #333;
}
</style>
