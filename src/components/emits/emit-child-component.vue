<template>
    <div  class="border-grey">
        Child Component Emits Example
        <button @click="$emit('emitData','raghuvar')">Click me to emit</button>
        
    </div>
</template>
<script>
export default {
    name: 'emitChildComponent',
    components : {
       
    },
    emits:['emitData'] ,
    data() {
        return {

        }
    }
}
</script>
<style>
</style>