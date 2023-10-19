<template>
  <div class="theSite">
    <portfolioHeader class="myHeader" />
    <portfolioContent class="myContent" />
    <portfolioFooter class="myFooter" />
  </div>
</template>

<script>
import PortfolioHeader from '@/components/portfolioHeader.vue';
import PortfolioContent from '@/components/portfolioContent.vue';
import PortfolioFooter from '@/components/portfolioFooter.vue';

export default {
  name: 'LandingPage',
  components: { PortfolioHeader, PortfolioContent, PortfolioFooter },
  props: {},
};
</script>

<style scoped>
.theSite {
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  padding: 10px;
}

.myHeader {
  display: flex;
  justify-self: flex-start;
  border: 1px solid red;
}
.myContent {
  display: flex;
  justify-items: stretch;
  border: 1px solid red;
}

.myFooter {
  display: flex;
  justify-self: flex-end;
  border: 1px solid red;
}
</style>
