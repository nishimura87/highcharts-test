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
          height: 300,
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
          data: [70, 70, 70, 70, 60, 60, 70, -20, -20, -20, 70, 50, 50, 50, 50, 70, 70, 70, 50, 70,]
        }],
        colors: ["#fff"],
      };
    },
  },
};
</script>
