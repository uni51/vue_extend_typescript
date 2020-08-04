<template></template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  computed: {
    // 戻り型アノテーションが必須
    greet(): string {
      return "Hello World!";
    },
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
