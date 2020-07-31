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
body {
  background-color: #ecf0f1;
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 60px;
}
</style>
