<template>
  <form action="" @submit.prevent="submitForm">
    <div>
      <label for="usrId">ID: </label>
      <input name="usrId" type="text" v-model="usrname">
    </div>
    <div>
      <label for="pwd">PWD: </label>
      <input type="password" name="pwd" v-model="pwd">
    </div>
    <button type="submit">로그인</button>
  </form>
</template>

<script>
// import 라이브러리명 from '패키지이름'
  import axios from 'axios'

  export default {
    data() {
      return {
        usrname: '',
        pwd: ''
      }
    },
    methods : {
      submitForm(){
//        event.preventDefault(); // $submit.prevent로 대체 (form submit의 기본동작 reload)

        const data = {
          username: this.usrname,
          password: this.pwd,
        }
        axios.post('https://jsonplaceholder.typicode.com/users', data) // sampleAPI:jsonplaceholder
          .then(response => {
            console.log(response);
          })
//        console.log('제출됨');
      }
    }
  }
</script>

<style lang="sass" scoped>

</style>