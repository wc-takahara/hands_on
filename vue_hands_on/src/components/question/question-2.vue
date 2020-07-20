<template>
  <!--
    【問題】
    変数count（初期値 0）をカウントアップしていってcountが偶数の場合に div leadの部分を非表示にしてください。

    使うVueの記法 v-on v-if
    使う関数名 countUp(カウントを増やして行く関数)
    ヒント 偶数かを判断する際には、変数 % 2 !== 0 と記載します。%2：2で割った際の余りが何かを求めるもの
   -->
  <div>
    <button>カウントアップするよ！</button>
    <div class="lead">count:{{count}}</div>
  </div>
</template>
<script>
export default {
  data: function() {
    return {
      count: 0,
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .lead {
    margin-top: 36px;
  }
</style>