<template>
  <highcharts :options="chartOptions"></highcharts>
</template>

<script>
export default {
  data() {
    return {};
  },
  computed: {
    chartOptions() {
      return {
        chart: {
          type: "column",
          backgroundColor: "black",
          borderColor: 'blue',
          borderRadius: 30,
          borderWidth: 2,
          inverted: true,
          height: 300,
        },
        title: {
          text: "Bar Chart3",
          style:{
            color: "#fff"
          }
        },
        xAxis: {
          gridLineWidth: 0,
          title:{
            text:''
          },
        },
        yAxis: {
          gridLineWidth: 0,
          title:{
            text:''
          },
          max: 100,
        },
        plotOptions: {
        },
        series: [{
          showInLegend: false,
          data: [80, 80, 80],
        }],
      };
    },
  },
};
</script>
