<template>
  <header>
    <nav>
      <ul>
        <li><nuxt-link class="header-link" to="/">Starting Page</nuxt-link></li>
        <li>
          <nuxt-link class="header-link" to="/recipes">Recipes</nuxt-link>
        </li>
        <li><nuxt-link class="header-link" to="/about">About</nuxt-link></li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
header {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: black;
  padding: 10px;
  margin-bottom: 20px;
}

ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}

li {
  margin: 0 10px;
  text-decoration: none;
  color: #fff;
}

.header-link {
  text-decoration: none;
  color: #fff;
  text-transform: uppercase;
  margin: 10px;
}

.header-link:hover {
  color: grey;
}
</style>
