<template>
  
  <parentRef/>
  <!-- 
  <tabsComp/>    
  <slotData/>
  <InputField v-model="name"/>
  <emitParentComponent/>
  <componentFirst/>
  <componentA/>
  <parentComponent/>
  <watcherThree/>
  <watcherTwo/>
  <WatcherComp/>
  <Userform/>
  
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
import Userform from './components/forms/Userform.vue';

import WatcherComp from './components/watchers/watcher-comp.vue';
import watcherTwo from './components/watchers/watcher-two.vue';
import watcherThree from './components/watchers/watcher-three.vue';
import parentComponent from './components/props/parent-component.vue';
import componentA from './components/provide-inject/component-a.vue';
import componentFirst from './components/provide-inject/component-first.vue';
import emitParentComponent from './components/emits/emit-parent-component.vue';
import InputField from './components/custom-model/InputField.vue';
import slotData from './components/slots/slot-component.vue';
import tabsComp from './components/dynamic-component/tabs-comp.vue';
*/
import parentRef from './components/refs/parent-ref.vue';



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
    Userform,
    WatcherComp,
    watcherTwo,
    watcherThree,
    parentComponent,
    componentA,
    componentFirst,
    emitParentComponent,
    InputField
    slotData,     
    tabsComp
    */    
    parentRef
  },
  data() {
    return {
      name: ''
    }
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
.full-border ,.border-grey {
 border: 1px solid #2c3e50;
 padding: 1rem;
 margin:1rem 0;
}

.card-wrapper {
  width: 400px;
  margin:1rem;
  border: 1px solid #2c3e50;
  padding: 1rem;
}

</style>
