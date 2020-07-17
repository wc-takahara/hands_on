<template>
  <button v-on:click="buttonAlert">クリック</button>
</template>
<script>
export default {
  methods:{
    buttonAlert: function(){
      alert('押したよ');
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>