<template>
  <div>
    <button v-on:click="classChange">色を変えるよ！</button>
    <div id="text" v-bind:class="toggleClass">テスト</div>
  </div>
</template>
<script>
export default {
  data: function() {
    return {
      toggleClass: 'red',
    }
  },
  methods: {
    classChange: function() {
      if(this.toggleClass == 'red'){
        this.toggleClass = 'blue';
      }else {
        this.toggleClass = 'red';
      }
    }
  }
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