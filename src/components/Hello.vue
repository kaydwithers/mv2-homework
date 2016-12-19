<template>
  <div id="hello">
    <h1>{{ msg }}</h1>
    <p class="mb3">A collection of homework from the excellent book, the Majesty of Vue.js 2</p>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Vue Homework'
    }
  }
}
</script>
 
<style scoped>
#hello {
  text-align: center;
  margin-top: 60px;
}
</style>
