<template lang="html">
  <div>
    <h1>This is the child component</h1>
    <div v-for="(individual, index) in people" :key="index">
      <span>{{ index+1 }}.   {{ individual.name }}</span>
    </div>
    <div>
      <h1> <a href="https://github.com/shanegibney/Vue-Passing-Data-From-Parent-To-Child-Component">Return to repo</a> </h1>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Child',
  props: ['people'],
  data(){
    return {}
  }
}
</script>

<style lang="css">
h1 {
   color: #444;
}
</style>
