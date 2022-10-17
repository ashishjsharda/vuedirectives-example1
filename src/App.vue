<template>
  <div id="app">
   <h1 v-text="title">Exercise 4</h1>
    <h2 v-html="html"></h2>
  </div>
</template>

<script>


export default {
  data(){
    return{
      title: 'CSS Module Component',
      subtitle: 'This is forth exercise',
      html: 'Stylise</br> HTML in </br> Vue Components',
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
