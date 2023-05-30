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
          type: "pie",
          backgroundColor: "black",
          borderColor: "blue",
          borderRadius: 30,
          borderWidth: 2,
        },
        title: {
          text: "Pie Chart",
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
        },
        plotOptions: {
          pie: {
            startAngle: -90,
            endAngle: 90,
            center: ['50%', '75%']
          }
        },
        series: [
          {
            showInLegend: false,
            innerSize: "90%",
            data: [20, 40],
          },
        ],
        colors: ["blue","purple"],
      };
    },
  },
};
</script>
