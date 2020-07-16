<template>
    <div>
        <label><input type="checkbox" value="A" v-model="val">A</label>
        <label><input type="checkbox" value="B" v-model="val">B</label>
        <label><input type="checkbox" value="C" v-model="val">C</label>
        <p>{{ val }}</p>
    </div>
</template>
<script>
export default {
  data: function() {
    return {
      val: []
    }
  },
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>