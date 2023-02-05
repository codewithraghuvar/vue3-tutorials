<template>

  <Userform/>
  <!--
  <ComputedPropertyFirst/>
  <ComputedPropertySecond/>
  <Methods/>
  <Variable/>  
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <HeaderComp/>
  -->
</template>

<script>
/*
import HelloWorld from './components/HelloWorld.vue'
import HeaderComp from './components/HeaderComp.vue'
import Variable from './components/variables/Variable.vue';
import Methods from './components/methods/Methods.vue';
import ComputedPropertyFirst from './components/computed/ComputedPropertyFirst.vue';
import ComputedPropertySecond from './components/computed/ComputedPropertySecond.vue';
*/
import Userform from './components/forms/Userform.vue';

export default {
  name: 'App',
  components: {
    /*
    Variable,
    HeaderComp,
    HelloWorld,
    Methods,
    ComputedPropertyFirst,
    ComputedPropertySecond,
    */
    Userform
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
.full-border {
 border: 1px solid #2c3e50;
 padding: 1rem;
 margin:1rem 0;
}

</style>
