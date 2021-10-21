<template>
    <div>
        <p>{{userx}}</p>
        <input v-model="userx">
    </div>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  props: ['user'],
  data() {
    return {
      userx: this.user,
    };
  },
  methods: {
    hello() {
      console.log('hello');
    },
  },
});

</script>

<style scoped>
input {
    color: gray
}
</style>
