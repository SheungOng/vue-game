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
import buttonSfx from './assets/soundbyte/404772__owlstorm__retro-video-game-sfx-blast-off.wav';

export default {
  name: 'App',
  components: {
    'v-button': ButtonC,
    VideoB
  },
  setup() {
    let [play] = useSound(buttonSfx, { volume: 0.3 })

    return {
      play,
    }
  },
}
</script>
