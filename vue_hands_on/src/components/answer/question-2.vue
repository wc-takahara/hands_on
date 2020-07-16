<template>
  <div>
    <button v-on:click="countUp">カウントアップするよ！</button>
    <div class="lead" v-if="count%2">count:{{count}}</div>
  </div>
</template>
<script>
export default {
  data: function() {
    return {
      count: 0,
    }
  },
  methods: {
    countUp: function(){
      this.count++;
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .lead {
    margin-top: 36px;
  }
</style>