<template></template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  props: {
    value: [Number, String],
    requiredValue: {
      type: [Number, String],
      required: true,
    },
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
