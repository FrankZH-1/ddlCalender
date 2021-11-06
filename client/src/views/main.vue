<template>
  <div class="main">
    <SearchBar></SearchBar>
    <TaskTable></TaskTable>
    <div class="button-container">
      <div class="button" @mousedown="isCovered = !isCovered">
        <img class="icon" src="@/icons/add-icon.png" />
      </div>
      <div class="button hint">
        <img class="icon" src="@/icons/hint-icon.png" />
      </div>
    </div>
    <TaskDetail :cover="isCovered"></TaskDetail>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
// import HelloWorld from '@/components/HelloWorld.vue'; // @ is an alias to /src
import SearchBar from "/src/components/search-bar.vue";
import TaskTable from "/src/components/task-table.vue";
import TaskDetail from "/src/components/task-detail.vue";
@Options({
  components: {
    SearchBar,
    TaskTable,
    TaskDetail,
  },
  props: {
    cover: Boolean,
  },
})
export default class Main extends Vue {
  data() {
    return {
      isCovered: false,
    };
  }
}
</script>
<style scoped>
.main {
  width: 100%;
}

.button-container {
  display: flex;
  justify-content: flex-start;
  margin-top: 26px;
}
.button {
  height: 35px;
  width: 141px;
  margin: 15px;
  background-color: #3370ff;
  border-radius: 5px;
}
.button .hint {
  width: 129px;
}
.icon {
  width: 25px;
  height: 25px;
  margin: 5px 0 5px 5px;
}
</style>