<template>
    <div>
      Count :  {{ count  }}
      <button @click="count+=1">Increase Count</button>
      <button @click="count-=1">Decrease Count</button>
    </div>

</template>
<script>
export default {
    name: 'watcher-comp',
    data() {
        return {
            count : 0
        }
    },
    watch:{
        count(newValue, oldValue){
            console.log('old count value='+oldValue)
            console.log('new count value='+newValue)
        }
    }
}
</script>
<style lang="scss">
</style>