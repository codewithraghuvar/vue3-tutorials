<template>
    <div>
      First name : <input type="text" v-model="name.firstName"/>
      Last name : <input type="text" v-model="name.lastName"/>
      <button @click="itemList.push('Laptop')">Add new item</button>
    </div>

</template>
<script>
export default {
    name: 'watcher-comp',
    data() {
        return {
            name: {
                firstName : 'Raghuvar',
                lastName: 'Visht'
            },
            itemList:[]
        }
    },
    watch:{
        name:{
            handler(newValue){
            console.log('first name ='+newValue.firstName + '== lastname =='+ newValue.lastName)
            },
            deep: true
        },
        itemList:{
            handler(newValue){
                console.log('itemlist ' + newValue)
            },
            deep: true
        }

    }
}
</script>
<style lang="scss">
</style>