<template>
  <div id="app">
    <img src="./assets/logo.png">
    <hello-world v-bind="{ ...barfoo, foobar }" />
  </div>
</template>

<script>
import HelloWorld from '@/components/HelloWorld'
export default {
  name: 'app',
  components: {
    HelloWorld
  },
  data () {
    return {
      barfoo: {
        foo: 'FOO',
        bar: 'BAR',
      },
      foobar: 'FOOBAR'
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
