<template>
    <div>
        <input :value="modelValue" @input="$emit('update:modelValue',$event.target.value)"/>
    </div>
</template>
<script>
export default {
    name:'InputField',
    props:{
        modelValue: String // modelValue this is the  use the same else it will not work
    }

}
</script>
<style>
</style>
