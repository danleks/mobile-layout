<template>
  <div id="app">
    <div class="wrapper">
      <app-mobile />
    </div>
  </div>
</template>

<script>
import Mobile from './components/Mobile.vue';


export default {
  name: 'app',
  components: {
    'app-mobile': Mobile,
  },
};
</script>

<style lang="scss">

html {
  box-sizing: border-box;
}
*, *:before, *:after {
  box-sizing: inherit;
  padding: 0;
  margin: 0;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

body {
  background-image: linear-gradient(to bottom right, #3c3eb1, #5ee87f);
}

.wrapper {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
