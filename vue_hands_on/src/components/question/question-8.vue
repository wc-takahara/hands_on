<template>
  <!--
    【問題】
     v-forを使ってリストを作成し、
　  「削除」ボタンを押したらリストから削除できるようにしてください

    使うVueの記法　v-for　v-on　
  　使う関数名　addList(input要素に記載した値をおぶジェクトに加える関数)
　　ヒント　削除する時の引数としてはindexを用いてください。(現在のリストが何番目かを保存している変数)
           配列から要素を削除する際は、下記メソッドが便利です。　配列.splice(配列の先頭から何番目か, 何個の要素を削除するか)
   -->
  <div>
    <ul>
      <li>スライム<button>削除</button></li>
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