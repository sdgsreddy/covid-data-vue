<template>
    
        <div>
        <div class = "dummy1">
            <div class = "dummy2">
            <p>COUNTRY: {{stateData.country}} </p>
            <p>STATE : {{stateData.state}} </p>
            <p>POPULATION: {{stateData.population}} </p>
            <p>COVID Positive cases: {{stateData.tested_positive}} </p>
            <p>INFECTION RATE: {{stateData.infection_rate}} </p>
            <p>HEADROOM COUNT_COVID ICU: {{stateData.icu_headroom_covid}} </p>
            <p>HEADROOM COUNT_NONCOVID ICU: {{stateData.icu_headroom_noncovid}} </p>
            <p>ACTUAL CASES: {{stateData.actual_cases}} </p>
            <p>ACTUAL DEATHS: {{stateData.actual_deaths}} </p>
            </div>
            <div class = "dummy3">
            <p>ACTUAL POSITIVE CASES: {{stateData.actual_positive_cases}} </p>
            <p>ACTUAL NEGATIVE CASES: {{stateData.actual_negative_cases}} </p>
            <p>TOTAL HOSPITAL BEDS: {{stateData.hospital_beds}} </p>
            <p>HOSPITAL BEDS USAGE: {{stateData.hospital_beds_usage}} </p>
            <p>HOSPITAL BEDS COVID: {{stateData.hospital_beds_covid}} </p>
            <p>TOTAL ICU BEDS: {{stateData.icu_beds}} </p>
            <p>ICU BEDS USAGE: {{stateData.icu_beds_usage}} </p>
            <p>ICU BEDS COVID: {{stateData.icu_beds_coivd}} </p>
            <p>VACCINCES DISTRIBUTED: {{stateData.vaccines_distributed}} </p>       
            <p>VACCINCES INITIATED: {{stateData.vaccines_intitiated}} </p>
            </div>
            
        </div>
        <hr>
    </div>
    
</template>

<script>
export default {
    name:'StateCovidData',
    props:{
        stateData: Object
    }
}
</script>

<style scoped>
.dummy1{
    display: inline-flex;
    background-color: yellowgreen;
    width: 100vw;
    font-weight: bold;
}
.dummy2{
    width: 50vw;
    margin-left: 50px;
}
</style>