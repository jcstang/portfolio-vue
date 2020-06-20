<template>
  <div id="app">
    <Nav url="./logo.png" />
    <Header msg="hello from the header comp" meImage="./headshot-trees-300x311.png" />
    <!-- <div class="container second-part">
      <h1>Hello!</h1>
    </div>-->
    <!-- <ListComp v-bind:items="items" /> -->
    <CardsContainer v-bind:items="items" />
    <ProjectsContainer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Nav from "./components/Nav.vue";
import CardsContainer from "./components/CardsContainer";
import ProjectsContainer from "./components/ProjectsContainer";
import "bulma/css/bulma.css";

export default {
  name: "App",
  components: {
    Header,
    Nav,
    CardsContainer,
    ProjectsContainer
  },
  data: function() {
    return {
      items: [
        { id: 1, message: "HTML", fontAwesomeIcon: "fab fa-html5 fa-2x" },
        { id: 2, message: "javaScript", fontAwesomeIcon: "fab fa-js fa-2x" },
        {
          id: 3,
          message: "CSS3",
          fontAwesomeIcon: "fab fa-css3 fa-2x"
        },
        {
          id: 4,
          message: "nodeJs",
          fontAwesomeIcon: "fab fa-node fa-2x"
        },
        {
          id: 5,
          message: "ReactJs",
          fontAwesomeIcon: "fab fa-react fa-2x"
        },
        {
          id: 6,
          message: "Vuejs",
          fontAwesomeIcon: "fab fa-vuejs fa-2x"
        }
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
