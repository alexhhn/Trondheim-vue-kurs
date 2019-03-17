<template>
  <div id="app">
    <CV/>
  </div>
</template>

<script>
import CV from "./components/CV.vue";

export default {
  name: "app",
  components: {
    CV
  }
};
</script>

<style>
body {
  background-color: #bed6e3;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  display: flex;
  justify-content: center;
}
</style>
