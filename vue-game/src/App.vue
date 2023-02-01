<template>
  <VideoB/>
  <div class="content">
    <h1 class="mb-5">Game Title</h1>
    <v-button :onClick="play">Start Game</v-button>
  </div>
</template>

<script>
import ButtonC from './components/ButtonC';
import VideoB from './components/VideoB';
import useSound from 'vue-use-sound';
import buttonSfx from './assets/soundbyte/243020__plasterbrain__game-start.ogg';

export default {
  name: 'App',
  components: {
    'v-button': ButtonC,
    VideoB
  },
  setup() {
    const [play] = useSound(buttonSfx)

    return {
      play,
    }
  },
}
</script>
