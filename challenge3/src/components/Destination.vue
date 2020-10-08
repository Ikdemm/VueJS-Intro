<template>
  <div id="destination">
    <div class="location-contain">
      <div class="locations">
        <div class="place">
          <img :src="location.img" width="235" height="300" />
          <h2>{{ location.name }}</h2>
          <p>
            {{ location.desc }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Destination",
  props: ["location"],
  data() {
    return {};
  },
};
</script>

<style scoped>
body {
  width: 100vw;
  height: 100vh;
  font-family: "NTR", sans-serif;
  background: #eee;
}

h1 {
  text-align: center;
}

.location-contain {
  display: -webkit-box;
  display: flex;
  -webkit-box-pack: center;
  justify-content: center;
}

.place {
  display: -webkit-box;
  display: flex;
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
  flex-direction: column;
  width: 280px;
  height: 320px;
  -webkit-box-pack: center;
  justify-content: center;
  background: white;
  border: 1px solid #ddd;
  padding: 20px 20px;
  margin: 10px;
}
.place h2 {
  margin: 0;
  text-align: center;
}
.place img {
  margin: 10px;
  align-self: center;
}
</style>