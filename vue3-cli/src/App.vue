<!-- HTML -->
<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<!-- JavaScript-->
<script>
// import 라이브러리 from '라이브러리이름'
// import 파일이름 from './파일경로'
import HelloWorld from './components/HelloWorld.vue'

export default {
  // 인스턴스 옵션 속성
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<!-- CSS -->
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
