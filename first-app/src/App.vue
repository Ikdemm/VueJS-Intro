<template>
  <div id="app">
    <Calculator />
    <Framework />
  </div>
</template>

<script>
import Framework from "./components/Framework.vue";
import Calculator from "./components/Calculator.vue";

export default {
  name: "App",
  data() {},
  components: {
    Framework,
    Calculator,
  },
};
</script>

<style>
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
