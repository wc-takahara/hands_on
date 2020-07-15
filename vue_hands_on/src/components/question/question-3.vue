<template>
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