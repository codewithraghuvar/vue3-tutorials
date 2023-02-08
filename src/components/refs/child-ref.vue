<template>
    <div>
     Chil Component
     Name <input type="text" ref="nameRef" v-model="name"/>
    </div>
</template>
<script>
export default {
    name: 'child-ref',
    data() {
        return {
            name:''
        }
    },
    methods:{
        callFromParent(){
            console.log('called from parent')
            this.name = 'Raghuvar'
        }
    }
}
</script>
<style>
</style>