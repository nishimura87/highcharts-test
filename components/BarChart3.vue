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
          column: {
            fillColor: {
                pattern: {
                    path: {
                        d: 'M 0 0 L 10 10 M 9 -1 L 11 1 M -1 9 L 1 11',
                        strokeWidth: 3
                    },
                    width: 10,
                    height: 10,
                    opacity: 0.4
                }
            }
        }
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
