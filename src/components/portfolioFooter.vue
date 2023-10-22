<template>
  <div class="portfolioFooter">
    <div>
      <li>GitHub Link</li>
    </div>
    <span>&copy;2023 - Erik Holman</span>
    <div>
      <li>Resume Link</li>
    </div>
  </div>
</template>

<script>
export default {
  name: 'portfolioFooter',
  props: {},
};
</script>

<style scoped>
.portfolioFooter {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
  width: auto;
  overflow: hidden;
}

.portfolioFooter li {
  list-style-type: none;
  text-align: center;
  border: 2px solid red;
  padding: 0;
  margin: 0;
}

.portfolioFooter li:hover {
  display: flex;
  color: white;
  background-color: darkblue;
  border-radius: 25px;
  text-transform: uppercase;
  cursor: grab;
}

.portfolioFooter span {
  font-family: 'Courier New', Courier, monospace;
  font-size: 20px;
  font-weight: 700;
  padding: 0;
  margin: 0;
}
</style>
