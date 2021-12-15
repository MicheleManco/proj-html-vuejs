<template>
  <div id="app">
    <div class="bg-color">
      <MyHeader/>
      <MyJumbotron/>
    </div>
    <MyMain/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MyFooter from './components/MyFooter.vue'
import MyMain from './components/MyMain.vue'
import MyJumbotron from './components/MyJumbotron.vue'

export default {
  name: 'App',
  components:{
    MyHeader,
    MyFooter,
    MyMain,
    MyJumbotron
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.bg-color{
  background-color: #f8f9fc;
}

</style>
