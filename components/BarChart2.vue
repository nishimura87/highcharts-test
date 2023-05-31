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
          borderColor: "blue",
          borderRadius: 30,
          borderWidth: 2,
          height: 300,
        },
        title: {
          text: "Bar Chart2",
          style: {
            color: "#fff",
          },
        },
        xAxis: {
          gridLineWidth: 0,
          title: {
            text: "",
          },
        },
        yAxis: {
          gridLineWidth: 0,
          title: {
            text: "",
          },
          max: 100,
        },
        plotOptions: {
          column: {
            stacking: "normal",
          },
        },
        series: [
          {
            showInLegend: false,
            data: [40, 30, 20],
            index:1,
          },
          {
            showInLegend: false,
            color: "#fff",
            data: [60, 70, 80],
            index:0
          },
        ],
      };
    },
  },
};
</script>
