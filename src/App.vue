<template>
  <LandingPage />
</template>

<script>
import LandingPage from './views/LandingPage';

export default {
  name: 'App',
  components: {
    LandingPage,
  },
};
</script>

<style>
body {
  padding: 0;
  margin: auto;
  overflow: hidden;
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
