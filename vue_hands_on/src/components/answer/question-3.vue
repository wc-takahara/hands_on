<template>
  <ul>
    <li v-for="item in list"
      v-bind:key="item.id">
      ID.{{ item.id }} {{ item.name }} HP.{{ item.hp }}
      <span v-if="item.hp > 300">つよい！</span>
    </li>
  </ul>
</template>
<script>
export default {
  data: function() {
    return {
      list: [
        { id: 1, name: 'スライム', hp: 100 },
        { id: 2, name: 'ゴブリン', hp: 200 },
        { id: 3, name: 'ドラゴン', hp: 500 }
      ]
    }
  },
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  ul {
    width: 500px;
    margin: 0 auto;
    text-align: start;
  }
</style>