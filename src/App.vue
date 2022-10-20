<template>
  <div id="app">
   <h1 v-if ="false" v-text="title">Loading</h1>
    <h2 v-else-if="false" v-html="html"></h2>
    <a
    v-else
    :href="link.url"
    :target="link.target"
    :tabindex="link.tabindex"
    v-text="link.title"

    />
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
