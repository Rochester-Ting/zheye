<template>
  <div class="container">
    <column-list :list="testData" />
  </div>
</template>
<script lang="ts">
/* eslint-disable */
import { defineComponent } from "vue";
import "bootstrap/dist/css/bootstrap.min.css";
import ColumnList from "./components/ColumnLIst.vue";
const testData = [
  {
    id: 1,
    title: "test1专栏",
    description:
      "test1专栏test1专栏test1专栏test1专栏test1专栏test1专栏test1专栏test1专栏test1专栏",
    avatar:
      "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=1546500353,2204894501&fm=26&gp=0.jpg",
  },
  {
    id: 2,
    title: "222",
    description: "大声叫道撒谎巨大商机的哈撒娇的哈市叫的撒和加大上级的哈市",
    avatar:
      "https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=1546500353,2204894501&fm=26&gp=0.jpg",
  },
];
export default defineComponent({
  name: "",
  props: {},
  components: {
    ColumnList,
  },
  setup() {
    return {
      testData,
    };
  },
});
</script>
<style scoped lang="scss"></style>
