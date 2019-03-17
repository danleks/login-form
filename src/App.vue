<template>
  <div id="app">
    <app-video/>
    <app-claim />
    <form action="#" class="inputWrapper">
        <app-input
      v-for="input in inputs"
      :key="input.id"
      :input="input"
      />
    </form>
    <app-button />
    <app-terms />
  </div>
</template>

<script>
import VideoBg from './components/VideoBg.vue';
import Claim from './components/Claim.vue';
import Input from './components/Input.vue';
import Terms from './components/Terms.vue';
import Button from './components/Button.vue';


export default {
  name: 'app',
  components: {
    'app-claim': Claim,
    'app-input': Input,
    'app-terms': Terms,
    'app-button': Button,
    'app-video': VideoBg,
  },

  data() {
    return {
      inputs: [
      {
        id: 1,
        type: 'email',
        icon: 'fa-user',
      },
      {
        id: 2,
        type: 'password',
        icon: 'fa-unlock-alt',
      }
    ]
    }
  }
};
</script>

<style lang="scss">
:root {
  --zIndex-init: -1;
  --zIndex-1: 100;
  --zIndex-2: 200;
  --zIndex-3: 300;
  --zIndex-4: 400;
  --zIndex-5: 500;
}
html {
  box-sizing: border-box;
  font-size: 62.5%;
}

body {

  @media(min-width: 1024px) {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
}
*, *:before, *:after {
  box-sizing: inherit;
  padding: 0;
  margin: 0;
}

#app {
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: 80rem;
  height: 100vh;
  margin: auto;
  background-color: rgba(#393B41, .5);
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  @media(min-width: 1024px) {
    height: 60rem;
    width: 60rem;

  }
}

.inputWrapper {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 90%;
}
</style>
