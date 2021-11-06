<template>
  <div class="search-box">
    <img class="search-icon" src="@/icons/search-icon.png" />
    <input class="search-input" />
    <el-select class="search-filter year"></el-select>
    <el-select class="search-filter month"></el-select>
    <el-select class="search-filter day"></el-select>
  </div>
</template>
<script lang="ts">
import { Options, Vue } from "vue-class-component";
@Options({})
export default class SearchBar extends Vue {}
</script>
<style scoped>
.search-box {
  width: 100%;
  height: 25px;
  top: 78px;
  margin-left: auto;
  margin-right: auto;
  /* background-color: aquamarine; */
  display: flex;
  justify-content: space-around;
  z-index: 1;
}
.search-icon {
  width: 25px;
  height: 25px;
  background-color: #ffffff;
}
.search-filter {
  width: 75px;
  height: 25px;
  border: 1px;
  background-color: #e3e9f9;
}
.search-input {
  width: 75px;
  height: 20px;
  background-color: #e3e9f9;
  border: none;
}
.search-input:active {
  border: none;
}
.search-filter >>> .el-input {
  line-height: 25px;
}
.search-filter >>> .el-input__inner {
  line-height: 25px;
  height: 25px;
}
</style>




