<template>
  <div id='app'>
    <Omikuji />
  </div>
</template>

<script>
import Omikuji from './components/Omikuji.vue';

export default {
  name: 'App',
  components: {
    Omikuji,
  },
};
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
