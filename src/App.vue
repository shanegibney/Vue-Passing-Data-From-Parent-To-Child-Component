<template>
  <div id="app">
    <h1>I am the parent component</h1>
    <Child :people="people"/>
  </div>
</template>

<script>
import Child from './components/Child'
export default {
  name: 'App',
  components: {
    Child
  },
  data(){
    return {
      title: 'People',
      people: [
        {name: 'Joe', qualified: 'false', reg: '123'},
        {name: 'Jill', qualified: 'true', reg: '231'},
        {name: 'June', qualified: 'false', reg: '312'},
        {name: 'Jack', qualified: 'true', reg: '132'}
      ]
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
