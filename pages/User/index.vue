<template>
  <div>
    <h1>New User Page</h1>

    <input type="number" v-model="userId" />
    <button @click="onLoadUser">Load User</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: "",
    };
  },

  methods: {
    onLoadUser() {
      this.$router.push("/user/" + this.userId);
    },
  },
};
</script>

<style scoped>
</style>