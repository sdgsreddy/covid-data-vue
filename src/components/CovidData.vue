<template>
    
    <div class="guna_1">
    <div v-for="stateData in statesData" :key="stateData._id">
        
        <StateCovidData :stateData="stateData"></StateCovidData>
    </div>
    </div>
</template>

<script>

import StateCovidData from './StateCovidData.vue';
export default {
    name:'CovidData',
    props:{
        statesData: Array
    },
    components:{
        StateCovidData
    }
}
</script>

<style scoped>

</style>