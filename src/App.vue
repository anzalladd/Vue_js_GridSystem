<template>
  <div id="app">
    <Content/>
  </div>
</template>

<script>
import Nav from './components/nav';
import Content from './components/content'
export default {
  
  name: 'app',
  components:{
    Nav,
    Content
  },

  }

</script>

<style>
*,body{
margin: 0;
padding: 0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
}

</style>
