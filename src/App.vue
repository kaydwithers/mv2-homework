<template>

  <div id="app">
    <hello></hello>

    <toggle name="one">
      <p>Hello 1</p>
    </toggle>

    <toggle name="two">
      <p>Hello 1</p>
    </toggle>

    <one></one>
    <two></two>
    <three></three>
    <four></four>

    <pre>
      {{ $data }}
    </pre>
  </div>

</template>

<script>
import Hello from './components/Hello.vue'
import Toggle from './components/Toggle.vue'
import One from './components/01.vue'
import Two from './components/02.vue'
import Three from './components/03.vue'
import Four from './components/04.vue'

export default {
  name: 'app',
  components: {
    Hello,
    Toggle,
    One,
    Two,
    Three,
    Four
  }
}
</script>

<style>
  body {
    color: #2b2b2b;
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    font-size: 14px;
    margin: 0 auto;
    padding: 1rem;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    width: 1280px;
  }

  label {
    display: block;
    font-size: 12px;
    margin-bottom: .5rem;
  }

  input, select {
    padding: .5rem;
  }

  h1, h2, h3, h4, h5, h6 {
    font-weight: normal;
  }

  ul {
    padding-left: 0;
  }

  li {
    list-style: none;
    margin-bottom: .5em;
  }

  .db {
    display: block;
  }

  .mb1 {
    margin-bottom: 1rem;
  }

  .mb2 {
    margin-bottom: 2rem;
  }

  .mb3 {
    margin-bottom: 3rem;
  }
</style>
