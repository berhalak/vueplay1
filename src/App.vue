<template>
  <div id="app">
    <list :items="items" />
  </div>
</template>

<script>
import List from './List.vue'

export default {
  name: 'app',
  components: {
    List
  },
  mounted(){
    window.app = this;
  },
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
      items : [1,2,3,4]
    }
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
