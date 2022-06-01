<template>
  <div>
    <div>count: {{ count }}</div>
    <div>count.value: {{ count.value }}</div>
    <button type="button" @click="count += 1">+</button>
    <button type="button" @click="count = '100'">set '100'</button>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from '@vue/composition-api';

const x: 0 = 1;

export default defineComponent({
  name: 'App',
  setup() {
    const count = ref(0);

    return {
      count,
    };
  }
});
</script>
