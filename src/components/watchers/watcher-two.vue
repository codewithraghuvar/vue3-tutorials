<template>
    <div>
      First name : <input type="text" v-model="firstName"/>
      Last name : <input type="text" v-model="lastName"/>
    </div>

</template>
<script>
export default {
    name: 'watcher-comp',
    data() {
        return {
            firstName : 'Raghuvar',
            lastName: 'Visht'
        }
    },
    watch:{
        firstName:{
            handler(newValue){
            console.log('first name ='+newValue)
            },
            immediate: true // use this when you want to check on component load
        },
        
        lastName(newValue){
            console.log('last name='+newValue)
        }

    }
}
</script>
<style lang="scss">
</style>