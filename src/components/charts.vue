<template>
    <ve-line :data="chartData" :settings="chartSettings"></ve-line>
</template>

<script>
export default {
  data() {
    this.chartSettings = {
      stack: { 用户: ['访问用户', '下单用户'] },
      area: true,
    };
    return {
      chartData: {
        columns: ['日期', '访问用户', '下单用户', '下单率'],
        rows: [
          {
            日期: '1/1', 访问用户: 1393, 下单用户: 1093, 下单率: 0.32,
          },
          {
            日期: '1/2', 访问用户: 1303, 下单用户: 1043, 下单率: 0.42,
          },
          {
            日期: '1/3', 访问用户: 1193, 下单用户: 1023, 下单率: 0.31,
          },
          {
            日期: '1/4', 访问用户: 1693, 下单用户: 1095, 下单率: 0.22,
          },
          {
            日期: '1/5', 访问用户: 1333, 下单用户: 1011, 下单率: 0.52,
          },
        ],
      },
    };
  },
};
</script>
