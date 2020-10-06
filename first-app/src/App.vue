<template>
  <div id="app">
    <div class="row">
      <input type="text" v-model.number="num1" />
      <span>+</span>
      <input type="text" v-model.number="num2" />
      <span>=</span>
      <span>{{ num1 + num2 }}</span>
    </div>
    <div class="row second">
      <select v-model="name">
        <option v-bind:key="framework" v-for="framework in frameworks">
          {{ framework }}
        </option>
      </select>
      <p>My favorite kind of taco is {{ name }}</p>
    </div>
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  data() {
    return {
      num1: 0,
      num2: 0,
      name: "React",
      frameworks: ["Angular", "React", "Vue"],
    };
  },
  // components: {
  //   HelloWorld
  // }
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
