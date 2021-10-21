<template>
    <p>{{count}}</p>
    <button v-on:click="increment">increment</button>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count += 1;
    },
  },
});
</script>
