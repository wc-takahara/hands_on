<template>
  <div>
    <div><input type="text" v-model="name"><button v-on:click="addList">追加</button></div>
    <ul>
      <li v-for="item in list"
        v-bind:key="item.id">{{ item.name }}</li>
    </ul>
  </div>
</template>
<script>
export default {
  data: function() {
    return {
      name: "",
      list: [
        { id: 1, name: 'スライム'},
        { id: 2, name: 'ゴブリン',},
        { id: 3, name: 'ドラゴン',}
      ]
    }
  },
  methods: {
    addList: function() {
      this.list.push({id: this.list.length, name: this.name});
      this.name = "";
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