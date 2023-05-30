<template>
  <div class="chart">
    <div class="chart_con">
      <BarChart />
    </div>
    <div class="chart_con">
      <BarChart2 />
    </div>
    <div class="chart_con">
      <BarChart3 />
    </div>
    <div class="chart_con">
      <AreaChart />
    </div>
    <div class="chart_con">
      <PieChart />
    </div>
  </div>
</template>

<style>
.chart {
  display:flex;
  justify-content:center;
  flex-wrap:wrap;
  background:black;
}

.chart_con {
  width:45%;
  margin:1%;
}
</style>