<template>
    <div>
     Tab C Content
     First name<input type="text" v-model="firstname"/>
    </div>
</template>
<script>
export default {
    name: 'TabC',
    data() {
        return {
            firstname:''
        }
    }
}
</script>
<style>
</style>