<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <div>
      <h5>Dibuat oleh Riki Widiantoro | link repository : <a href="https://github.com/rikiwidiantoro/ecommerce-catalog" target="_blank">https://github.com/rikiwidiantoro/ecommerce-catalog</a></h5>
    </div>
    <ProductDisplay/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import ProductDisplay from './components/ProductDisplay.vue'

export default {
  name: 'app',
  components: {
    ProductDisplay
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
body {
  background: linear-gradient(to bottom, #D6E6ff 50%, #FDE2FF 50%);
  /* background-color: #FDE2FF; */
}
</style>
