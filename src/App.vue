<template>
  <div id="app">
    <MyHeader/>
    <MyFooter/>
    <MyMain/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyFooter from './components/MyFooter.vue'
import MyMain from './components/MyMain.vue'
export default {
  name: 'App',
  components:{
    MyHeader,
    MyFooter,
    MyMain
  }
}
</script>

<style lang="scss">

</style>
