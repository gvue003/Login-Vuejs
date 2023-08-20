<template>
  <button class="logout-button" @click="logout">Logout</button>
</template>

<script>
export default {
  methods: {
    logout() {
      this.$router.push('/');
    }
  }
};
</script>

<style>
</style>
