<template>
  <div id="app">
    <my-header></my-header>
    <h1>{{ headmsg }}</h1>
    <my-footer></my-footer>
    <my-content></my-content>
    <my-content2></my-content2>
  </div>
</template>

<script>
import header from './myComponent/Header.vue'
import footer from './myComponent/Footer.vue'
import content from './myComponent/Content.vue'
import content2 from './myComponent/Content2.vue'
export default {
  name: 'app',
  components:{
    "my-header" : header,
    "my-footer" : footer,
    "my-content" : content,
    "my-content2" : content2
  },
  data () {
    return {
      headmsg: 'Welcome My Header'
    }
  }
}
</script>

<style>
#app {
 
  text-align: center;
  
}

</style>
