<template>
  <!--
    【問題】
    ボタンを押すたびに #textのdiv要素が赤色と青色に切り替わるようにしてください。

    使うVueの記法 v-on v-bind
    使う関数名 classChange(#textにつけるclass名を切り替える関数)
    ヒント 色の切り替えは用意してあるクラスを使用してください。(赤色の場合は：red,青色の場合は：blue)
          変数toggleClassに上記のクラス名(どちらか)を格納してください。それを上記の関数で現状変数toggleClassに格納されているクラスがどちらなのかを精査して、redだったらblue、blueだったらredに切り替えてください。
   -->
  <div>
    <button>色を変えるよ！</button>
    <div id="text">テスト</div>
  </div>
</template>
<script>
export default {
  data: function() {
  },
  methods: {
  },
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