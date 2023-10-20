<template>
  <!-- <ehLoader /> -->
  <LandingPage />
</template>

<script>
// import EhLoader from './components/ehLoader.vue';
import LandingPage from './views/LandingPage';

export default {
  name: 'App',
  components: {
    LandingPage,
    // EhLoader,
  },
};
</script>

<style>
html,
body {
  height: 100%;
}

body {
  display: flex;
  flex-direction: column;
  padding: 0;
  margin: auto;
  overflow: hidden;
}

.portfolioContent {
  flex: 1 0 auto;
}

.portfoliofooter {
  flex-shrink: 0;
}

.ehLoader {
  display: unset;
  position: relative;
  transition: all 10s;
}

#app {
  font-family: Arial, Helvetica, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-size: 14px;
  color: black;
  background-color: darkgrey;
  height: 100vh;
}
</style>
