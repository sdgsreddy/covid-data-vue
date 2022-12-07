<template>
  <div>
    <div class = "dummy">COVID DATA ANALYSIS</div>
    <a href="https://proud-tan-tank-top.cyclic.app/about">About Me</a>
    <CovidData :statesData = "statesData"></CovidData>
  </div>
</template>

<script>

import CovidData from './components/CovidData.vue';
import axios from 'axios';
export default {
  name : 'App',
  components: {
    CovidData
  },
  data() {
    return {
      statesData:[]
    }
  },
  methods:{
    async getCovidDataAnalysis() {
      const response = await axios.get("https://proud-tan-tank-top.cyclic.app/covid",{
        mode:'no-cors',
        referrerPolicy : 'origin',
      });
      return response.data;
    }
  },

  async created() {
    this.statesData = await this.getCovidDataAnalysis();
  }
}
</script>

<style>
.dummy{
    text-align: center;
    font-size:  xx-large;
    background-color: aquamarine;
    font-weight: bolder;
    height: 40px;
    margin-bottom: 10px;
    padding: 40px;
}
</style>
