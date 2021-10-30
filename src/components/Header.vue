<template>
    <h1 :style="styles">Welcome {{name}} how are you</h1>
</template>

<script>

export default {
  data() {
    return {
      styles: {
        color: 'blue',
        fontSize: '50px',
      },
      name: 'Brenden',
    };
  },
};
</script>

<style scoped>
h1 {
    color: gray
}
</style>
