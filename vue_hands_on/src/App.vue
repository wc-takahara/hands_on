<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
     <h3>ハンズオン</h3>
    <question/>
  </div>
</template>

<script>
import question from './components/question/question-8.vue'

export default {
  name: 'App',
  components: {
    question
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
