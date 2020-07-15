<template>
    <div>
        <label><input type="checkbox" value="A"> A</label>
        <label><input type="checkbox" value="B"> B</label>
        <label><input type="checkbox" value="C"> C</label>
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