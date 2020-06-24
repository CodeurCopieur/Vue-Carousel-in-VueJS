<template>
  <div id="app">
    <Slider></Slider>
  </div>
</template>

<script>
import Slider from './components/includes/Slider'

export default {
  name: 'App',
  components: {
    Slider
  }
}
</script>

<style lang="scss">

@import url('./assets/scss/index.scss');

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

div div button {
  outline: none;
}
</style>
