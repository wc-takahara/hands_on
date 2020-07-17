<template>
  <!--
    【問題】
    .v-forを使ってリストを作成し、
　  さらにinputからでリストに追加する名前を入力し、「追加」ボタンを押したら、リストに追加されるようにしてください。

    使うVueの記法　v-for　v-on　v-model　
  　使う関数名　addList(input要素に記載した値をおぶジェクトに加える関数)
　　ヒント　オブジェクトのの最後尾に要素を加える場合は、push()メソッドを使いましょう。
           追加した後は、v-modelで使っている変数を初期化してあげると使い勝手が良いかもです。
   -->
  <div>
    <div><input type="text"><button>追加</button></div>
    <ul>
      <li>スライム</li>
      <li>ゴブリン</li>
      <li>ドラゴン</li>
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