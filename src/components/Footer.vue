<template>
    <div>
        <p>{{newuser}}</p>
        <input v-model="newuser">
    </div>
</template>

<script>
// <Footer user="Hello" />
export default {
  props: ['user'],
  data() {
    return {
      newuser: this.user,
    };
  },
};
</script>
