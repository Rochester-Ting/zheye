<template>
  <div class="container">
    <global-header :user="user" />
    <column-list :list="testData" />
  </div>
</template>
<script lang="ts">
/* eslint-disable */
import { defineComponent } from "vue";
import "bootstrap/dist/css/bootstrap.min.css";
import ColumnList from "./components/ColumnLIst.vue";
import GlobalHeader from "./components/GlobalHeader.vue";
// import { UserProps } from "./components/GlobalHeader.vue";
const testData = [
  {
    id: 1,
    title: "test1专栏",
    description:
      "test1专栏test1专栏test1专栏test1专栏test1专栏test1专栏test1专栏test1专栏test1专栏",
    avatar:
      "http://oss.runnerbar.com/img/watermark/user_upload/origin/20210313/1615634961038_3939e95e_9d4e_4243_9414_8c45f9092447.JPG",
  },
  {
    id: 2,
    title: "222",
    description: "大声叫道撒谎巨大商机的哈撒娇的哈市叫的撒和加大上级的哈市",
    avatar:
      "http://oss.runnerbar.com/img/watermark/user_upload/origin/20210313/1615634961038_3939e95e_9d4e_4243_9414_8c45f9092447.JPG",
  },
  {
    id: 3,
    title: "3",
    description: "大声叫道撒谎巨大商机的哈撒娇的哈市叫的撒和加大上级的哈市",
    avatar:
      "http://oss.runnerbar.com/img/watermark/user_upload/origin/20210313/1615634961038_3939e95e_9d4e_4243_9414_8c45f9092447.JPG",
  },
  {
    id: 4,
    title: "4",
    description: "大声叫道撒谎巨大商机的哈撒娇的哈市叫的撒和加大上级的哈市",
    avatar:
      "http://oss.runnerbar.com/img/watermark/user_upload/origin/20210313/1615634961038_3939e95e_9d4e_4243_9414_8c45f9092447.JPG",
  },
  {
    id: 5,
    title: "222",
    description: "大声叫道撒谎巨大商机的哈撒娇的哈市叫的撒和加大上级的哈市",
    avatar:
      "http://oss.runnerbar.com/img/watermark/user_upload/origin/20210313/1615634961038_3939e95e_9d4e_4243_9414_8c45f9092447.JPG",
  }
];
export default defineComponent({
  name: "",
  props: {},
  components: {
    ColumnList,
    GlobalHeader
  },
  setup() {
    const user = {
      isLogin: false,
      name: 'roct',
      id: 15737
    }
    return {
      testData,
      user
    };
  },
});
</script>
<style scoped lang="scss"></style>
