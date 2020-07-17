<template>
  <!--
    【問題】
    用意したリストを、ul要素の中に表示する。(key は id)
　  それが完了したら、hpが300以上の場合には<span>つよい！</span> を表示させてください。

    使うVueの記法　v-for  v-if
  　使う関数名　関数使わない
　　ヒント　v-forの中でv-if使います。
   -->
  <ul>
    <!-- この中にリストの値をそれぞれ表示する -->
　　<!-- 例： ID.1  スライム　HP.100 -->
　　<!-- 例： ID.2  ゴブリン　HP.200 -->
    <!-- 例： ID.3  ドラゴン　HP.500  つよい！-->
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