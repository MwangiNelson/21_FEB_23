<script>
    import ProfileVue from './ProfileVue.vue';
</script>
<template>
  <nav class="app-navbar">
    <div class="nav-links">
      <a href="">HOME</a>
      <a href="">ABOUT</a>
      <a href="">PROFILE</a>
    </div>
    <div class="nav-profile">
      <ProfileVue />
    </div>
  </nav>
</template>


<style scoped>
.app-navbar {
  width: 100%;
  height: fit-content;
  background-color: blueviolet;
  display: flex;
  justify-content: center;
  align-items: center;
  position: fixed;
  top: 0;
  left: 0;
}
.nav-links {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  justify-items: center;
  width: 50%;
  color: white;
  text-transform: uppercase;
}
.nav-profile {
  position: relative;
  right: 10%;
}
</style>
