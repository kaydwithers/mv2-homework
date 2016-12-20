<template>
  <div class="mb3">
    <h2>Simple Calculator (@click)</h2>

    <div class="mb1">
      <input type="number" v-model.number="a">
      <select v-model="operator">
        <option>+</option>
        <option>-</option>
        <option>*</option>
        <option>/</option>
      </select>
      <input type="" v-model.number="b">
    </div>

    <div class="mb1">
      <button @click.prevent="calculate">Calculate</button>
      <h4>Result: {{a}} {{operator}} {{b}} = {{c}}</h4>
    </div>

  </div>
</template>



<script>
  export default {
    data () {
      return {
        a: 1,
        b: 2,
        c: null,
        operator: '+',
      }
    },
    methods: {
      calculate: function() {
        switch (this.operator) {
          case '+':
            this.c = this.a + this.b
            break;
          case '-':
            this.c = this.a - this.b
            break;
          case '*':
            this.c = this.a * this.b
            break;
          case '/':
            this.c = this.a / this.b
            break;
        }
      }
    }
  }
</script>



<style scoped>

</style>
