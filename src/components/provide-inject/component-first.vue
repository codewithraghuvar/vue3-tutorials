<template>
    <div>
        component first
        Username in First component {{ name }}
        <componentSecond/>
    </div>
</template>
<script>
import componentSecond from './component-second.vue';
export default {
    name: 'component-first',
    components : {
        componentSecond
    },
    data() {
        return {
            name: 'Raghuvar'
        }
    },
    provide () {
        return {
            username: this.name
        }        
    }
}
</script>
<style>
</style>