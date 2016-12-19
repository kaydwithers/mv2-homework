<template>
  <div class="mb3">
    <h2>List rendering</h2>

    <div class="mb1">
      <ul>
        <li v-for="(value, key, index) in values">
          {{ index }}: {{ key }} = {{ value }}
        </li>
      </ul>
    </div>

  </div>
</template>



<script>
  export default {
    data () {
      return {
        values: {
          name: 'Kayd',
          height: '186cm',
          weight: 'N/A',
          eyeColor: 'Green',
          favoriteFood: 'Pizza',
        }
      }
    }
  }
</script>



<style scoped>

</style>
