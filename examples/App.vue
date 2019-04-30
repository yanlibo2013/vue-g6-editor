<template>
  <div id="container">
    <BaseFlow :data="data" :getData="save"/>
  </div>
</template>

<script>
/* eslint-disable */
import BaseFlow from '../packages/vue-g6-editor/src/BaseFlow.vue'
import FlowData from "./model/flow";

export default {
  name: "app",
  data() {
    return {
      data: FlowData
    };
  },
  components: {
    BaseFlow
  },
  methods: {
    save() {}
  }
};
</script>

<style lang="scss">
#container {
  font-family: "Helvetica Neue", Helvetica, "PingFang SC", "Hiragino Sans GB",
    "Microsoft YaHei", "微软雅黑", Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  height: 100%;
}
* {
  box-sizing: border-box;
  margin: 0px;
}
</style>
