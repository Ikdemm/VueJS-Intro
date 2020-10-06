<template>
  <div class="row">
    <input type="text" v-model.number="num1" />
    <span>+</span>
    <input type="text" v-model.number="num2" />
    <span>=</span>
    <span>{{ num1 + num2 }}</span>
  </div>
</template>

<script>
export default {
  name: "Calculator",
  props: {},
  data() {
    return {
      num1: 0,
      num2: 0,
    };
  },
};
</script>