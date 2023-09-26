<template>
  <div id="app">
    <InputCreate />
  </div>
</template>

<script>
import InputCreate from './components/InputCreate.vue'

export default {
  name: 'App',
  components: {
    InputCreate
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
</style>
