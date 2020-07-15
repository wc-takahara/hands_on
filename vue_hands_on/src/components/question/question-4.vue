<template>
  <div>
    <button>色を変えるよ！</button>
    <div id="text">テスト</div>
  </div>
</template>
<script>
export default {
  data: function() {
  },
  methods: {
  },
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #text {
    margin-top: 36px;
  }
  #text.red {
    color: red;
  }
  #text.blue {
    color: blue;
  }
</style>