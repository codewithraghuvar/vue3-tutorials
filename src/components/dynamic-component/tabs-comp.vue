<template>
    <div>
        <button @click="activeTab= 'TabA'">Tab A</button>
        <button @click="activeTab= 'TabB'">Tab B</button>
        <button @click="activeTab= 'TabC'">Tab C</button>
        <!--
        <TabA v-if="activeTab === 'TabA'"></TabA>
        <TabB v-if="activeTab === 'TabB'"></TabB>
        <TabC v-if="activeTab === 'TabC'"></TabC>
        -->
        <!--keep alive keep dynamic component alive-->
        <KeepAlive>
        <component :is="activeTab"/>
        </KeepAlive>
    </div>
</template>
<script>
import TabA from './TabA.vue';
import TabB from './TabB.vue';
import TabC from './TabC.vue'
export default {
    name: 'tabs-comp',
    components:{
        TabA,
        TabB,
        TabC
    },
    data() {
        return {
             activeTab: 'TabA'
        }
    }
}
</script>
<style>
</style>