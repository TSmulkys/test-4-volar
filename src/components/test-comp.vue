<template lang="pug">
p {{ text }}
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'TestComp',
  props: {
    text: {
      type: String,
      required: true
    }
  },
  setup() {
    return {
      //
    };
  },
});
</script>

<style scoped lang="postcss"></style>
