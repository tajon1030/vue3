<template>
  <div>
    {{ msg }}
  </div>
  <button @click="showAlert">경고</button>
</template>

<script>
  export default {
    data() {
      return {
        msg: 'hi'
      }
    },
    methods :{
      showAlert(){
        alert('hello');
      }
    }
  }
</script>

<style scoped>

</style>