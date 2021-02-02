<template>
  <div class="home">
    <div class="btn" @click=" visible = true ">Open</div>
    <div class="btn" @click=" visible = false ">Close</div>
    <MumuDrawer title="Title" v-model="visible" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import MumuDrawer from "@/components/common/index.vue";

@Component({
  components: {
    MumuDrawer,
  },
})
export default class Home extends Vue {
  private visible: boolean = false;
}
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
