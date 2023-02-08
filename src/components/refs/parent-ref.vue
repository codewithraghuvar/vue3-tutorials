<template>
    <div>
     Parent Ref
     Name <input type="text" v-model="name" ref="nameRef"/>
     <childRef ref="childCompRef"/>
    </div>
</template>
<script>
import childRef from './child-ref.vue'
export default {
    name: 'parent-ref',
    components:{
        childRef
    },
    data() {
        return {
            name:''
        }
    },
    mounted(){
        this.$refs.nameRef.focus()

        this.$refs.childCompRef.callFromParent()
       console.log(this.$refs.childCompRef)
    }
}
</script>
<style>
</style>