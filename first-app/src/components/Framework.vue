<template>
  <div class="row second">
    <select v-model="name">
      <option v-bind:key="framework" v-for="framework in frameworks">
        {{ framework }}
      </option>
    </select>
    <p>My favorite kind of taco is {{ name }}</p>
  </div>
</template>

<script>
export default {
  name: "Framework",
  props: {},
  data() {
    return {
      name: "React",
      frameworks: ["Angular", "React", "Vue"],
    };
  },
};
</script>

