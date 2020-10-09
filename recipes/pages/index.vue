<template>
  <div class="container">
    <h1>Welcome to Recipeez!</h1>
    <p>
      Here you can find the best and easiest Recipeez to make during Quarantine
    </p>
    <button class="jump-button">
      <nuxt-link to="/recipes" class="jump-link">Jump right in!</nuxt-link>
    </button>
  </div>
</template>

<script>
import Header from '@/components/Header'

export default {}
</script>

<style scoped>
.container {
  padding: 10px;
}

* {
  text-align: center;
}

.jump-button {
  background-color: peru;
  color: white;
  border: 2px solid white;
  border-radius: 5px;
  padding: 10px;
  margin-top: 15px;
}

.jump-button:hover {
  background-color: rgb(179, 139, 30);
  cursor: pointer;
}

.jump-link {
  color: white;
  text-decoration: none;
  text-transform: uppercase;
  font-weight: bold;
}
</style>
