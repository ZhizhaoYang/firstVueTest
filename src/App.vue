<template>
  <div id="app">
    <div class="row">
      <input v-model.number="num1" type="number">
      <span>+</span>
      <input v-model.number="num2" type="number">
      <span>=</span>
      <span>{{ num1 + num2 }}</span>
    </div>
    <div class="row second">
      <select v-model="name">
        <option>Cat</option>
        <option>Dog</option>
        <option>Monkey</option>
        <option>Mouse</option>
      </select>
      <p v-if="name">My favorite kind of animal is {{ name }}</p>
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

// export default {
//   name: "app",
//   components: {
//     HelloWorld
//   }
// };

export default {
  name: "#app",
  data() {
    return {
      num1: 0,
      num2: 0,
      name: ""
    };
  }
};
</script>

<style>
/* #app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
@import "./App.css";
</style>
