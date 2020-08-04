<template></template>

<script lang="ts">
import Vue, { PropType } from "vue";

export default Vue.extend({
  // この方法では、親コンポーネントから与えられるpropsが誤っていても、コンパイルエラーを得ることができません
  props: {
    obj: {
      type: Object as PropType<{ name: string }>,
      required: true,
    },
    arr: {
      type: Array as PropType<{ task: string }[]>,
    },
  },
  computed: {
    myName(): string {
      return this.obj.name;
    },
    myFirstTask(): string {
      return this.arr[0].task;
    },
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
