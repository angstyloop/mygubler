<template>
  <div id="app">
    <img alt="Matthew Gray Gubler" src="./assets/mgg.jpg">
    <div class="text">{{quotes[0]}}</div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      quotes: [
        "You came and I was crazy for you, and you cooled my mind that burned with longing.",
        "Love shook my heart like the wind on the mountain rushing over the oak trees.",
      ]
    }
  },
}
</script>

<style>
#app {
  width: 100vw;
  height: 100vh;
  background-color: black !important;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #2c3e50;
  position: relative;
  margin: 0;
  border: 0;
  padding: 0;
}
.text { 
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 10%;
  position: absolute;
  font-size: 4vh;
  color: white;
  width: auto;
}
img {
  align-self: flex-start;
  opacity: .7;
  width: auto;
  max-width: 100%;
  height: auto;
}
</style>
