<template>
  <div class="cover" :class="{ covered: cover }">
    <div class="task-detail"></div>
  </div>
</template>

<script >
import { Options, Vue } from "vue-class-component";
import {watch} from "vue";
@Options({
  props: {
    cover: Boolean,
  },
})
export default class TaskDetail extends Vue {
  setup(props,ctx){
    const info = props.cover;
    watch(info,(newVal){

    })
  }
}
</script>

<style scoped>
.cover {
  display: none;
  position: absolute;
  width: 100%;
  height: 100%;
  margin: -10px;
  z-index: 2;
  display: flex;
}
.covered {
  display: block;
  backdrop-filter: blur(4px);
}
</style>>
