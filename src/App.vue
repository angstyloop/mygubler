<template>
  <div id="app">
    <div class="text">
        <span>{{quote}}</span>
    </div>
    <img alt="Matthew Gray Gubler" src="./assets/mgg.jpg">
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      quotes: [
        ["Not knowing when the dawn will come, I open every door.", "Emily Dickenson"],
        ["Where thou art, that is home.", "Emily Dickenson"],
        ["You came and I was crazy for you, and you cooled my mind that burned with longing.", "Sappho"],
        ["Love shook my heart like the wind on the mountain rushing over the oak trees.", "Sappho"],
      ]
    }
  },
  computed: {
    quote() {
      return this.quotes[0][0] || ""
    }
  }
}
</script>

<style>
body {
  background-color: black !important;
  display: flex;
  align-items: center;
  justify-content: center;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  max-width: 1000px;
}
.text { 
  font-size: 4vh;
  padding: 1vh;
  color: white;
}
img {
  opacity: .75;
  width: auto;
  max-width: 100%;
  height: auto;
}
</style>
