<template>
  <div id="app">
    <!-- <h1>Your Upcoming Destinations</h2> -->
    <div class="location-contain">
      <div class="locations">
        <div class="place">
          <img
            src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/28963/moscow.svg"
            width="235"
            height="300"
          />
          <h2>Moscow</h2>
          <p>
            Moscow is the capital and most populous city of Russia, with 13.2
            million residents within the city limits and 17.8 million within the
            urban area. Moscow has the status of a Russian federal city.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
};
</script>

<style>
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
