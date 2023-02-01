<template>
  <div id="app">
    <h1 class="mb-5">Game Title</h1>
    <v-button :onClick="play">Start Game</v-button>
  </div>
</template>

<script>
import ButtonC from './components/ButtonC';
import useSound from 'vue-use-sound';
import buttonSfx from './assets/soundbyte/243020__plasterbrain__game-start.ogg';

export default {
  name: 'App',
  components: {
    'v-button': ButtonC
  },
  setup() {
    const [play] = useSound(buttonSfx)
    
    return {
      play,
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
