<template>
  <div class='omikuji-app'>
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
      result: 'Vueおみくじ',
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
