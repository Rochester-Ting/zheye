<template>
  <nav class="navbar navbar-light bg-light mb-4 bg-primary">
    <a class="navbar-brand" href="#">者也专栏</a>
    <ul v-if="!user.isLogin">
      <li class="list-inline-item">
        <a href="#" class="btn btn-outline-primary my-2">登录</a>
      </li>
      <li class="list-inline-item">
        <a href="#" class="btn btn-outline-primary my-2">注册</a>
      </li>
    </ul>
    <ul v-if="user.isLogin">
      <li class="list-inline-item">
        <a href="#" class="btn btn-outline-primary my-2">你好{{user.name}}</a>
      </li>
    </ul>
  </nav>
</template>

<script lang="ts">
import { defineComponent, PropType } from 'vue';
export interface UserProps {
  isLogin: boolean;
  name?: string;
  id?: number;
}
export default defineComponent({
  name: 'GlobalHeader',
  props: {
    user: {
      type: Object as PropType<UserProps>,
      require: true
    }
  },
  components: {},
  setup() {
    return {};
  }
});
</script>

<style scoped lang="scss"></style>
