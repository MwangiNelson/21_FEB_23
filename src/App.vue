<script setup>
import Navigation from "./components/Navigation.vue";
import Profile from "./components/Profile.vue";
</script>

<template>
  <Navigation />
  <div class="nav-profile">
    <Profile />
  </div>
</template>

<style scoped>
.nav-profile {
  position: absolute;
  right: 10%;
  top: 0%;
}
</style>
