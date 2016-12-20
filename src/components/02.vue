<template>
  <div class="mb3">
    <h2>Template (v-if)</h2>

    <div v-if="gender == 'male' || gender == 'female'">
      <h3>
        Hello 
        <span v-show="gender == 'male'">Mister</span> 
        <span v-show="gender == 'female'">Miss</span>
        {{ nameFirst }}
      </h3>
    </div>

    <div v-else="gender == ''">
      <h3>Hello {{ nameFirst }}</h3>
    </div>

    <div class="mb1">
      <label for="gender">Enter Your gender</label>
      <input name="gender" type="text" v-model="gender" />
    </div>

    <div class="mb1">
      <label for="nameFirst">Enter Your Name</label>
      <input name="nameFirst" type="text" v-model="nameFirst" />
    </div>

  </div>
</template>



<script>
  export default {
    data () {
      return {
        gender: 'female',
        nameFirst: 'Wellington'
      }
    }
  }
</script>



<style scoped>

</style>
