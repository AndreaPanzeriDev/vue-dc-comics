<template>
  <div id="app">
    
    <HeaderComp/>
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp
  }
}
</script>

<style lang="scss">

body{
  background-color: #1f1f1f;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}

</style>
