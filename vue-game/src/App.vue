<template>
  <div id="app">
    <h1 class="mb-5">Game Title</h1>
    <v-button :onClick="logClick">Start Game</v-button>
  </div>
</template>

<script>
import ButtonC from './components/ButtonC';

export default {
  name: 'App',
  components: {
    'v-button': ButtonC
  },
  methods: {
    logClick() {
      console.log('Game has started')
    }
  },
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
