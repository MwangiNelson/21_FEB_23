<script></script>
<template>
  <nav class="app-navbar">
    <div class="nav-links">
      <a href="">HOME</a>
      <a href="">ABOUT</a>
      <a href="">PROFILE</a>
    </div>
  </nav>
</template>

<style scoped>
.app-navbar {
  width: 100%;
  padding-block: 3.5vh;
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
  width: 25%;
  text-transform: uppercase;
}
.nav-links a {
  color: white;
}
</style>
