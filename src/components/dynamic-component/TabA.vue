<template>
    <div>
     Tab A Content
     Name <input type="text" v-model="name"/>
    </div>
</template>
<script>
export default {
    name: 'TabA',
    data() {
        return {
            name:''
        }
    }
}
</script>
<style>
</style>