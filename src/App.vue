<template lang="pug">
div(class="app-class")
  TestComp(:text="loremText")
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'

// Components
import TestComp from "./components/test-comp.vue";

export default defineComponent({
  name: 'App',
  components: { TestComp },
  setup() {
    const loremText = ref('Lorem ipsum dolor, sit amet consectetur adipisicing elit. Officia, quaerat? Incidunt, rem fugiat a deserunt aliquam qui vel quidem. Deleniti nihil est rerum, eius adipisci mollitia dicta amet distinctio inventore?')

    return {
      loremText
    }
  }
})
</script>

<style scoped lang="postcss">
.app-class {
  background-color: pink;
}
</style>
