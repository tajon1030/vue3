<template>
  <form action="">
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
  export default {
    data() {
      return {
        usrname: '',
        pwd: ''
      }
    },
  }
</script>

<style lang="sass" scoped>

</style>