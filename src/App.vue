<template>
  <div id="app">
    <Header></Header>
    <Events></Events>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Events from './components/Events.vue';

export default {
  name: 'App',
  components: {
    Header,
    Events,
  },
};
</script>

<style lang="scss">
#app {
  font-family: "Montserrat", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #ffffff;
  overflow: hidden;
  display: flex;
  justify-content: space-between;
  background: linear-gradient(rgba(4, 33, 73, 0.7) 100%, rgba(4, 33, 73, 0.5) 100%),
    url("./assets/main-background.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  width: 100vw;
  max-width: 100%;
  height: 100vh;
  max-height: 100%;
  background-position: center left;
}
</style>
