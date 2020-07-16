<template>
  <button v-on:click="buttonAlert">クリック</button>
</template>
<script>
export default {
  methods:{
    buttonAlert: function(){
      alert('クリックしたよ');
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>