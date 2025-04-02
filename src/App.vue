<script>
export default {
  data() {
    return {
      num : 0
    };
  },
  methods: {
    decreasement () {
      this.num -= 1
    },
    increasement (e) {
      this.num += 1
    },
  }
};

</script>

<template>
  <h1 v-text="num"></h1>
  <button v-on:click="decreasement">감소</button>
  <button @click="$event => increasement($event)">증가</button>
</template>

<style>

</style>
