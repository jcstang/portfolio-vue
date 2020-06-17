<template>
  <div id="app">
    <Nav url="./logo.png" />
    <Header
      msg="hello from the header comp"
      meImage="./headshot-trees-300x311.png"
    />
    <div class="container second-part">
      <h1>Hello!</h1>
    </div>
    <ListComp />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Nav from './components/Nav.vue';
import ListComp from './components/ListComp.vue';
import 'bulma/css/bulma.css';
// const listOfItems = [{ message: 'Foo' }, { message: 'Bar' }];

export default {
  name: 'App',
  components: {
    Header,
    Nav,
    ListComp,
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
.second-part {
  border: 1px solid red;
}
</style>
