<template>
  <div id="app">
    <!-- <Calculator /> -->
    <!-- <Framework /> -->
    <Users />
  </div>
</template>

<script>
// import Framework from "./components/Framework.vue";
// import Calculator from "./components/Calculator.vue";
import Users from "./components/Users.vue";

export default {
  name: "App",
  data() {
    return{}
  },
  components: {
    // Framework,
    // Calculator,
    Users
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.row {
  margin: 50px;
  display: -webkit-box;
  display: flex;
  -webkit-box-pack: center;
  justify-content: center;
  font-family: "Work Sans", sans-serif;
}

input,
span {
  padding: 10px;
  font-size: 30px;
  font-family: "Work Sans", sans-serif;
}

input {
  width: 50px;
}

span {
  width: 20px;
}

.second {
  font-size: 18px;
}
.second p {
  margin-left: 20px;
}
</style>
