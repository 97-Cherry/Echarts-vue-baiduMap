<template>
  <div ref="echarts" id="myDiv"></div>
</template>

<script>
import * as mycharts from 'echarts'
export default {
  mounted() {
    let myEcharts=mycharts.init(this.$ref.echarts);
    myEcharts.setOption({
      title:{
        text:'主标题',
        textStyle:{
          color:'#333'
        }
      }
    })
  },

}
</script>

<style>
#myDiv{
  width: 500px;
  height: 500px;
  border: 1px solid red;
}

</style>