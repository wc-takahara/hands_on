<template>
  <!--
    【問題】
    v-bindとv-onでv-modelを再現してください

    使うVueの記法　v-bind　v-on
  　使う関数名　関数使わない
　　ヒント　input要素で入力した値を取得するには  $event.target.value でできます。
   -->
    <div>
        <div>
            <input type="text" v-model="message">
            <div>v-modelを使う：{{message}}</div>
        </div>
        <div>
            <input type="text">
            <div>v-on,v-bindを使う：{{message1}}</div>
        </div>
    </div>
</template>
<script>
export default {
  data: function() {
    return {
      message: 'テスト',
      message1: 'テスト',
    }
  },
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>