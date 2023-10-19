<template>
  <div class="theSite">
    <portfolioHeader />
    <portfolioContent />
  </div>
</template>

<script>
import PortfolioHeader from '@/components/portfolioHeader.vue';
import PortfolioContent from '@/components/portfolioContent.vue';

export default {
  name: 'LandingPage',
  components: { PortfolioHeader, PortfolioContent },
  props: {},
};
</script>

<style scoped>
.theSite {
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  justify-content: space-between;
  padding: 10px;
}
</style>
