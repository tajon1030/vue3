<template>
  <AppHeader v-bind:appTitle="msg"
  v-on:change="changeTitle"></AppHeader>
</template>

<script>
// import 컴포넌트이름 from './컴포넌트 경로'
  import AppHeader from './components/AppHeader.vue'

  export default {
    components : {
      // '컴포넌트이름' : 컴포넌트 내용
      // 'app-header' : AppHeader // 네이밍컨벤션은 파스칼케이스
      // 'AppHeader' : AppHeader  // 컴포넌트이름은 어짜피 문자이기때문에 따옴표 생략
      // AppHeader : AppHeader // 앞뒤 같은 단어면 하나로 축약가능
      AppHeader
    },
    data() {
      return {
        msg: 'hi'
      }
    },
    methods :{
      showAlert(){
        alert('hello');
      },
      changeTitle(){
        this.msg = '클릭'
      }
    }
  }
</script>

<style scoped>

</style>