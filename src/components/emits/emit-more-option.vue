<template>
    <div  class="border-grey">
        More option emits Example
        <button @click="$emit('emitUser','Anshul')">Click me to emit</button>
        
    </div>
</template>
<script>
export default {
    name: 'emitChildComponent',
    components : {
       
    },
    emits:{
        emitUser: (name) => {
            return name;
        }
    },
    data() {
        return {

        }
    }
}
</script>
<style>
</style>