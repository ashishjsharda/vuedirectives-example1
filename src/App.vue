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
  data() {
    return {
      // v-text
      text: 'Directive text',
      // v-html
      html: 'Stylise</br>HTML in<br/><b>your data</b>',
      // v-bind
      link: {
        url: 'https://google.com',
        target: '_blank',
        tabindex: '0',
        title: 'Go to Google',
      },
    }
  },
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
