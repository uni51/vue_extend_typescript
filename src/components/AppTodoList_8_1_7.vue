<template></template>

<script lang="ts">
import Vue from "vue";

export type Todo = {
  id: string;
  task: string;
  done: boolean;
};

export type Data = {
  firstName: string;
  lastName: string;
  todos: Todo[];
};

export default Vue.extend({
  data: (): Data => ({
    firstName: "Taro",
    lastName: "Yamada",
    todos: [],
  }),
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
