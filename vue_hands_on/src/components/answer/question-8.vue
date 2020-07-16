<template>
  <div>
    <ul>
      <li v-for="(item, index) in list"
        v-bind:key="item.id">{{ item.name }}<button v-on:click="deleteList(index)">削除</button></li>
    </ul>
  </div>
</template>
<script>
export default {
  data: function() {
    return {
      list: [
        { id: 1, name: 'スライム'},
        { id: 2, name: 'ゴブリン',},
        { id: 3, name: 'ドラゴン',}
      ]
    }
  },
  methods: {
    deleteList: function(index) {
      console.log(index)
      this.list.splice(index, 1);
    }
  }
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