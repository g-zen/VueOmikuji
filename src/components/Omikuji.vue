<template>
  <div class='omikuji-app'>
    <h1 class="title">Vueおみくじ</h1>
    <h1 class='fortune'>{{ result }}</h1>
    <button class='btn'
            @click="drawFortune">おみくじを引く</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      fortunes: [
        '大吉',
        '吉',
        '凶',
        '大凶',
      ],
      result: '',
    };
  },
  methods: {
    drawFortune() {
      const index = Math.floor(Math.random() * this.fortunes.length);
      this.result = this.fortunes[index];
    },
  },
};
</script>

<style scoped>
  .omikuji-app {
    background-color: #34495e;
    border-radius: 10px;
    display: inline-block;
    font-family: Avenir, Helvetica, Arial, sans-serif;
    text-align: center;
    width: 300px;
  }
  .title {
    color: #fff;
  }
  .fortune {
    background-color: #fff;
    border-radius: 8px;
    display: block;
    height: 50px;
    margin: 15px;
  }
  .btn {
    display: block;
    background-color: #fff;
    height: 40px;
    margin: 15px;
    width: 90%;
  }
</style>
