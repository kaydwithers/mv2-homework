<template>

  <!--<button @click.prevent="toggle()">
    {{ toggleActive ? 'Hide ' + name : 'Show ' + name }}
  </button>

  <div v-show="toggleActive">
    <slot></slot>
  </div>-->

</template>



<script>
  export default {
    props: ['name'],
    data: function() { 
      return { 
        toggleActive: false
      }
    },
    methods: {
      toggle: function() {
        this.toggleActive = !this.toggleActive;
      }
    }
  }
</script>



<style scoped>

</style>
