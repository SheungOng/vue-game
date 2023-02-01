<template>
  <GameWorld title="Welcome to Your Game World App"/>
</template>

<script>
import GameWorld from './components/GameWorld.vue';

export default {
  name: 'App',
  components: {
    GameWorld
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
