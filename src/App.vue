<template>
  <div id="app">
    
    <HeaderComp/>
    <MainComp/>,
    <LinkComp/>
    <FooterComp/>
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import LinkComp from './components/LinkComp.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    LinkComp,
    FooterComp
  }
}
</script>

<style lang="scss">

body{
  background-color: #1f1f1f;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  padding: 0;
  height: 100vh;
  width: 100vw;
}

</style>
