<template></template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  data: () => ({
    firstName: "",
    lastName: "",
    doneTodos: null as null | boolean,
    todos: [] as Array<{
      id: string;
      task: string;
      done: boolean;
    }>,
  }),
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
