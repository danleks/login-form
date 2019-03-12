<template>
  <div id="app">
    <app-login />
    <app-claim />
    <div class="inputWrapper">
        <app-input
      v-for="input in inputs"
      :key="input.id"
      :input="input"
      />
    </div>
    <app-button />
    <app-terms />
  </div>
</template>

<script>
import Login from './components/Login.vue';
import Claim from './components/Claim.vue';
import Input from './components/Input.vue';
import Terms from './components/Terms.vue';
import Button from './components/Button.vue';



export default {
  name: 'app',
  components: {
    'app-login': Login,
    'app-claim': Claim,
    'app-input': Input,
    'app-terms': Terms,
    'app-button': Button,
  },

  data() {
    return {
      inputs: [
      {
        id: 1,
        type: 'email'
      },
      {
        id: 2,
        type: 'password'
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
*, *:before, *:after {
  box-sizing: inherit;
  padding: 0;
  margin: 0;
}

#app {
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 100vh;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.inputWrapper {
  flex: 1;
}
</style>
