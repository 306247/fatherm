<template>
  <div class="home">
    <div class="btn">Open</div>
    <div class="btn">Close</div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({
  components: {
  },
})
export default class Home extends Vue {}
</script>
<style lang="less" scoped>
.btn {
  display: inline-block;
  width: 100px;
  padding: 10px 0;
  margin: 0 16px;
  text-align: center;
  border: 1px solid #cccccc;
  border-radius: 4px;
}
</style>
