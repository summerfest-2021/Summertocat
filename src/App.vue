<template>
  <octocat/>
</template>

<script>
import Octocat from './components/Octocat.vue'

export default {
  name: 'App',
  components: {
    Octocat
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
