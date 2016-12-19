<template>
  <div class="mb3">
    <h2>Two way binding</h2>
    <h3>Hello {{ nameFull }}</h3>
    <label for="nameFull">Enter Your Name</label>
    <input name="nameFull" type="text" v-model="nameFull" />
  </div>
</template>



<script>
  export default {
    data () {
      return {
        nameFull: ''
      }
    }
  }
</script>



<style scoped>

</style>
