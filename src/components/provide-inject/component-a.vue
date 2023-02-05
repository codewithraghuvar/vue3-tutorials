<template>
    <div>
        component A
        username in Comp A {{ username }}
        <componentB/>
    </div>
</template>
<script>
import componentB from './component-b.vue';
export default {
    name: 'component-a',
    components : {
        componentB
    },
    data() {
        return {

        }
    },
    provide: {
        username: 'Raghuvar'
    }
}
</script>
<style>
</style>