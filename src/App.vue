<template>
  <div id="app">
    <Nav />
    <Header msg="hello from the header comp" />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Nav from './components/Nav.vue';
import 'bulma/css/bulma.css';

export default {
  name: 'App',
  components: {
    Header,
    Nav,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
