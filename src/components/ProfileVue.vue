<template>
  <div class="profile-photo">
    <img :src="ProfilePhoto" alt="" />
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
.profile-photo img{
  width: 5vw;
  height: 5vw;
  border-radius: 50%;
object-fit: cover;
}
</style>
