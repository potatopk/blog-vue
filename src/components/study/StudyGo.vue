<template>
  <el-table
    :data="tableData"
    style="width: 100%"
    :height="tableHeight"
  >
    <el-table-column
      prop="date"
      label="日期"
      width="180"
    >
    </el-table-column>
    <el-table-column
      prop="name"
      label="姓名"
      width="180"
    >
    </el-table-column>
    <el-table-column
      prop="address"
      label="地址"
    >
    </el-table-column>
  </el-table>
</template>

  <script lang="ts">
import { Vue, Component } from 'vue-property-decorator';

@Component
export default class StudyGo extends Vue {
  private tableData: object[] = [
    {
      date: '2016-05-02',
      name: '王小虎',
      address: '上海市普陀区金沙江路 1518 弄'
    },
    {
      date: '2016-05-04',
      name: '王小虎',
      address: '上海市普陀区金沙江路 1517 弄'
    },
    {
      date: '2016-05-01',
      name: '王小虎',
      address: '上海市普陀区金沙江路 1519 弄'
    },
    {
      date: '2016-05-03',
      name: '王小虎',
      address: '上海市普陀区金沙江路 1516 弄'
    }
  ];
  private tableHeight: number = 202;

  mounted() {
    this.tableHeight = 208;
  }
}
</script>
  