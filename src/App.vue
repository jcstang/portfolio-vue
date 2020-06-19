<template>
  <div id="app">
    <Nav url="./logo.png" />
    <Header msg="hello from the header comp" meImage="./headshot-trees-300x311.png" />
    <!-- <div class="container second-part">
      <h1>Hello!</h1>
    </div>-->
    <!-- <ListComp v-bind:items="items" /> -->
    <CardsContainer v-bind:items="items" />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Nav from "./components/Nav.vue";
import CardsContainer from "./components/CardsContainer";
import "bulma/css/bulma.css";

export default {
  name: "App",
  components: {
    Header,
    Nav,
    CardsContainer
  },
  data: function() {
    return {
      items: [
        { id: 1, message: "hi" },
        { id: 2, message: "goodbye" },
        { id: 3, message: "cool cool cool" },
        { id: 4, message: "today today" },
        { id: 5, message: "some stuff and other stuff" },
        { id: 6, message: "cool cool stuff a roooo" }
      ]
    };
  }
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
