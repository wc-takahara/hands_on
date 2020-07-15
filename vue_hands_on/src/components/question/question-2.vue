<template>
  <div>
    <button>カウントアップするよ！</button>
    <div class="lead">count:{{count}}</div>
  </div>
</template>
<script>
export default {
  data: function() {
    return {
      count: 0,
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