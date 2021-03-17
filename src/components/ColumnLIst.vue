<template>
  <ul v-for="item of list" :key="item.id">
    <img :src="item.avatar" alt="item.title" />
    <h5>{{ item.title }}</h5>
    <p>{{ item.description }}</p>
    <a href="#">进入专栏</a>
  </ul>
</template>

<script lang="ts">
import { defineComponent, PropType } from 'vue'
export interface ColumnProps {
  id: number;
  title: string;
  avatar: string;
  description: string;
}
export default defineComponent({
  name: 'ColumnList',
  props: {
    list: {
      type: Array as PropType<ColumnProps[]>,
      required: true
    }
  },
  components: {},
  setup () {
    return {}
  }
})
</script>

<style scoped lang="scss"></style>
