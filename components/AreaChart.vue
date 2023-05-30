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
          type: "area",
          backgroundColor: "black",
          borderColor: 'blue',
          borderRadius: 30,
          borderWidth: 2,
        },
        title: {
          text: "Bar Chart",
          style:{
            color: "#fff"
          }
        },
        xAxis: {
          gridLineWidth: 0,
          title:{
            text:''
          }
        },
        yAxis: {
          gridLineWidth: 0,
          title:{
            text:''
          }
        },
        plotOptions: {},
        series: [{
          showInLegend: false,
          data: [0, 30, 80, 10, 10, 50, 30,-20, 0, 10],
        }],
        colors: ["#fff"],
      };
    },
  },
};
</script>
