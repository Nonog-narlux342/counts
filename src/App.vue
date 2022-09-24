<template>
  <div id="app">
    <img alt="Profile" class="rounded-circle" src="./assets/1.jpg" Width="20%"/>
    <h1>Nonog_Narlux</h1>
    <h3>Images Score</h3>
    <hr />
    <div class="row">
      <div class="col">
        <img alt="Profile" class="rounded" src="./assets/3.jpg" Width="80%"/>
        <br />
        <br />
        <HelloWorld />
      </div>
      <div class="col">
        <img alt="Profile" class="rounded" src="./assets/5.jpg" Width="80%"/>
        <br />
        <br />
        <HelloWorld />
      </div>
      <div class="col">
        <img alt="Profile" class="rounded" src="./assets/6.jpg" Width="80%"/>
        <br />
        <br />
        <HelloWorld />
      </div>
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
  },
  data: function () {
    return {
      total: 0,
      name: "",
      code: "",
      gpa: 0.1,
    };
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
  margin-top: 60px;
}
</style>
