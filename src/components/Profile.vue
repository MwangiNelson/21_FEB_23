<template>
  <div class="profile-photo">
    <img :src="ProfilePhoto" alt="" />
    <span class="explanation"><p>This is Elliot Alderson</p></span>
  </div>
</template>

<script>
import ProfilePhoto from "../assets/hackerman.jpg";
export default {
  data() {
    return {
      ProfilePhoto,
    };
  },
};
</script>

<style scoped>
.profile-photo img {
  width: 5vw;
  height: 5vw;
  border-radius: 50%;
  object-fit: cover;
}

.profile-photo {
  display: flex;
  flex-direction: column;
}

.explanation {
  transform: translateY(15px) translateX(15px);
  background-color: rgb(56, 56, 56);
  color: white;
  border-radius: 4px;
  margin: 0;
  padding: 0.25em 0.75em;
  position: relative;
  display: flex;
  flex-direction: column;
  opacity: 0;
  transition: all 0.5s ease;
}
img:hover + .explanation {
  opacity: 1;
}
.explanation::before {
  content: "";
  background-color: rgb(56, 56, 56);
  height: 25px;
  z-index: 1;
  width: 25px;
  transform: rotate(45deg);
  position: absolute;
  top: -10%;
}
</style>
