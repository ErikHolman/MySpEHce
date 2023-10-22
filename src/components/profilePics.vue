<template>
  <img class="profilePics" :src="this.url" />
</template>

<script>
export default {
  name: 'profilePics',
  props: {
    url: String,
  },
};
</script>

<style scoped>
.profilePics {
  width: 400px;
  height: 400px;
  border: 8px solid white;
  background: attr(src);
  border-radius: 50%;
  background-repeat: no-repeat;
  background-position: center -60px;
  background-size: cover;
  box-shadow: 5px 5px rgba(0, 0, 0, 0.6);
}
</style>
