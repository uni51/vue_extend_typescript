<template>
  <div class="todos">
    <div v-for="todo in todos" :key="todo.id">
      <AppTodoItem :todo="todo" />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
// 親コンポーネントであるAppTodoListは、子コンポーネントであるAppTodoItemからTodo型をインポートする
import AppTodoItem, { Todo } from "./AppTodoItem.vue";

export type Data = {
  todos: Todo[];
};

export default Vue.extend({
  data: (): Data => ({
    todos: [],
  }),
  components: {
    AppTodoItem,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
