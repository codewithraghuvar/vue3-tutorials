<template>
    <div class="border-grey">
       Parent Component Emits Example 
       name: {{ name }}
        <emitChildComponent @emitData = "emitDataParent"/>
        <emitMoreOption @emitUser="emitUserData"/>
    </div>
</template>
<script>
import emitChildComponent from './emit-child-component.vue';
import emitMoreOption from './emit-more-option.vue';
export default {
    name: 'emitParentComponent',
    components : {
        emitChildComponent,
        emitMoreOption
    },
    data() {
        return {
            name: ''
        }
    },
    methods:{
        emitDataParent(value){
            this.name = value
            console.log('call emit in parent =' + value)
        },
        emitUserData(value) {
            console.log('value of user data = '+ value)
        }
    }
}
</script>
<style>
</style>