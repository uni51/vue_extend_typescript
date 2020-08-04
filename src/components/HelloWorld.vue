<template>
  <div @click="onClickElement">test</div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  data: () => ({
    bounds: null as ClientRect | DOMRect | null,
  }),
  methods: {
    onClickElement({ target }: { target: HTMLElement }): void {
      this.bounds = target.getBoundingClientRect();
    },
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
