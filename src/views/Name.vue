<template>
    <div>
        <p>Please enter your name</p>
        <input v-model="user">
        <button v-on:click="save">Save</button>
        <p v-if="user">Hello {{user}}</p>
    </div>
</template>

<script>
module.exports = {
  data() {
    return { user: 'Brenden' };
  },
  methods: {
    save() {
      console.log(this.user);
    },
  },
};
</script>
