<template>
  <div id="app">
    <img alt="Matthew Gray Gubler" src="./assets/mgg_1.jpg">
    <div class="text">{{quote}}</div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      quote: "Love shook my heart like the wind on the mountain rushing over the oak trees."
    }
  },
}
</script>

<style>
#app {
  background-color: black;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  position: relative;
  /*margin-top: 60px;*/
}
.text {
  position: absolute;
  bottom: 15%;
  font-size: 8vh;
  color: white;
  width: auto;
}
img {
  opacity: .8;
  width: auto;
  max-width: 100%;
  height: auto;
}
</style>
