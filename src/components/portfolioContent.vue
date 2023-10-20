<template>
  <div class="portfolioContent">
    <span class="titleName">Erik Holman</span>
    <div class="timeline">
      <div class="lines">&nbsp;</div>
      <div class="content">
        <div class="entry">
          <h3>Birth</h3>
          <span>Somewhere in the PNW, sometime in the later 1900s</span>
        </div>
        <div class="entry">
          <h3>College</h3>
          <span
            >Somewhere in the Phoenix Valley, sometime in the 20-oughts</span
          >
        </div>
        <div class="entry">
          <h3>MediaPRO</h3>
          <span>A clever blurb about the time at MediaPRO</span>
          <blockquote>a quote</blockquote>
        </div>
        <div class="entry">
          <h3>KnowBe4</h3>
          <span>A clever blurb about the time at KB4</span>
          <blockquote>a quote</blockquote>
        </div>
        <div class="entry">
          <h3>8Months, 17Days</h3>
          <span>A clever blurb about the time at MediaPRO</span>
          <blockquote>a quote</blockquote>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'portfolioContent',
  props: {},
};
</script>

<style scoped>
.portfolioContent {
  display: flex;
  flex-direction: column;
  width: auto;
  overflow-y: scroll;
  overflow-x: hidden;
  align-items: center;
  justify-content: center;
}

.timeline {
  padding: 20px;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}

.lines {
  display: flex;
  flex-direction: column;
  border-top: 0;
  border-right: 1px;
  border-bottom: 0;
  border-left: 0;
  border-color: white;
  border-style: solid;
  height: auto;
  width: 20px;
  justify-content: stretch;
  align-self: stretch;
}

.content {
  display: flex;
  flex-direction: column;
  padding-left: 10px;
}

.entry h3,
.entry span,
.entry blockquote {
  padding: 0;
  margin: 0;
  font-family: 'tilt neon';
}

.entry {
  padding-bottom: 30px;
}

.entry h3 {
  text-decoration: overline;
  text-decoration-color: white;
  border-left: 1px soild white;
}

.titleName {
  font-size: 10em;
  font-family: 'tilt neon';
}
</style>
