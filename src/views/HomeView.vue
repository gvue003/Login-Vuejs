<template>
  <div class="home-view">
    <div class="centered-content">
      <h1 class="home-title">Home Page</h1>
      <p>This is the Home Page</p>
      <logout-button></logout-button>
    </div>
  </div>
</template>

<script>
import LogoutButton from '@/components/LogoutButton.vue';

export default {
  components: {
    LogoutButton
  }
};
</script>

<style>
.home-view {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.centered-content {
  text-align: center;
}

.home-title {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 10px;
}
</style>
