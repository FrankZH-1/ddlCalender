<template>
  <div class="table">
    <el-table
      :data="tableData"
      :row-style="{ height: '70px' }"
      style="width: 100%"
      max-height="600px"
    >
      <el-table-column prop="date" label="日期" width="60%" />
      <el-table-column prop="all" label="全体成员" width="80%" />
      <el-table-column prop="product" label="产品组" width="80%" />
      <el-table-column prop="backend" label="服务端" width="80%" />
      <el-table-column prop="frontend" label="前端" width="80%" />
    </el-table>
  </div>
</template>
<script>
// import { defineComponent } from '@vue/composition-api'
import { Vue } from "vue-class-component";

export default class TaskTable extends Vue {
  data() {
    return {
      tableData: [
        {
          date: "周期任务",
          all: "",
          product: "",
          backend: "",
          frontend: "",
        },
        {
          date: "10.2",
          all: "",
          product: "",
          backend: "",
          frontend: "",
        },
        {
          date: "10.3",
          all: "",
          product: "",
          backend: "",
          frontend: "",
        },
        {
          date: "10.4",
          all: "",
          product: "",
          backend: "",
          frontend: "",
        },
        {
          date: "10.5",
          all: "",
          product: "",
          backend: "",
          frontend: "",
        },
        {
          date: "10.6",
          all: "",
          product: "",
          backend: "",
          frontend: "",
        },
        {
          date: "10.7",
          all: "",
          product: "",
          backend: "",
          frontend: "",
        },
        {
          date: "10.8",
          all: "",
          product: "",
          backend: "",
          frontend: "",
        },
        {
          date: "10.9",
          all: "",
          product: "",
          backend: "",
          frontend: "",
        },
      ],
    };
  }
  setup() {}
}
</script>
<style scoped>
.table {
  margin-top: 18px;
  z-index: 1;
}
</style>