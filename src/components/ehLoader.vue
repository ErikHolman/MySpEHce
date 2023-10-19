<template>
  <div class="ehLoader" v-if="isLoading">
    <img class="profilePic" src="../assets/profile.jpg" />
    <span>{{ this.isLoading }}</span>
  </div>
</template>

<script>
export default {
  name: 'ehLoader',
  props: { showLoader: Boolean },
  data() {
    return {
      // isLoading: this.showLoader,
      isLoading: true,
    };
  },
  mounted() {
    setTimeout(() => {
      this.isLoading = false;
    }, 6000);
  },
};
</script>

<style scoped>
.ehLoader {
}

.profilePic {
  width: 25%;
  transform: rotate(0.75turn);
}
</style>
