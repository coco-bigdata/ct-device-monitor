<template>
  <div class="bottom-right-table-1">
    <dv-border-box-6>
      <div class="table-name">
        <img src="./img/icon1.png" />人员贡献排行榜
      </div>

      <dv-scroll-board :config="config" />
    </dv-border-box-6>
  </div>
</template>

<script>
export default {
  name: 'BottomRightTable1',
  data () {
    return {
      config: {
        data: [
          ['铁塔员工1', '月累计排除故障：4起'],
          ['铁塔员工2', '月累计排除故障：3起'],
          ['铁塔员工3', '月累计排除故障：3起'],
          ['铁塔员工4', '月累计排除故障：3起'],
          ['铁塔员工5', '月累计排除故障：2起'],
          ['铁塔员工6', '月累计排除故障：2起'],
          ['铁塔员工7', '月累计排除故障：2起'],
          ['铁塔员工8', '月累计排除故障：2起'],
          ['铁塔员工9', '月累计排除故障：2起'],
          ['铁塔员工10', '月累计排除故障：2起']
        ],
        index: true,
        columnWidth: [30, 70],
        align: ['center'],
        oddRowBGC: 'rgba(9, 37, 50, 0.4)',
        evenRowBGC: 'rgba(10, 32, 50, 0.3)'
      }
    }
  }
}
</script>

<style lang="less">
.bottom-right-table-1 {
  width: calc(~"25% + 10px");
  height: 100%;
  margin: 0 -5px;

  .border-box-content {
    padding: 20px;
    box-sizing: border-box;
  }

  .table-name {
    height: 45px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 15px;

    img {
      width: 40px;
      height: 40px;
      margin-right: 5px;
    }
  }

  .dv-scroll-board {
    height: calc(~"100% - 60px");
  }
}
</style>
