<template>
  <div class="portfolioContent">
    <span class="titleName">Erik Holman</span>
    <div class="timeline">
      <div class="left">
        <profilePics url="../assets/profile.jpg" />
      </div>
      <div class="lines">&nbsp;</div>
      <div class="content">
        <div class="entry">
          <h3>Birth</h3>
          <span>Somewhere in the PNW in the later 1900s</span>
        </div>
        <div class="entry">
          <h3>College</h3>
          <span>Valley of the Sun sometime in the 20-oughts</span>
          <span>HIDDEN: 33.41638409460698, -111.9615222176947</span>
        </div>
        <div class="entry">
          <h3>MediaPRO</h3>
          <span>A clever blurb about the time at MediaPRO</span>
          <blockquote>
            a quote a quote a quote a quote a quote a quote a quote a quote a
            quote a quote a quote a quote a quote a quote a quote a quote a
            quote a quote a quote a quote a quote a quote a quote a quote a
            quote a quote a quote a quote a quote a quote a quote a quote a
            quote a quote a quote a quote a quote
          </blockquote>
        </div>
        <div class="entry">
          <h3>KnowBe4</h3>
          <span>A clever blurb about the time at KB4</span>
          <blockquote>a quote</blockquote>
        </div>
        <div class="entry">
          <h3>8Months, 17Days</h3>
          <span>A clever blurb about the time spent unemployed</span>
          <blockquote>a quote</blockquote>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import profilePics from './profilePics.vue';
export default {
  components: { profilePics },
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
  height: auto;
}

.left {
  display: flex;
  flex-direction: column;
  width: 50vw;
  justify-content: stretch;
  align-items: stretch;
}

.lines {
  display: flex;
  width: 3px;
  height: 75vh;
  background-color: white;
  align-content: stretch;
  align-items: center;
  flex-wrap: wrap;
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
  padding-bottom: 15px;
}
.entry::before {
  content: '';
  display: inline-block;
  position: relative;
  height: 10px;
  width: 10px;
  border-radius: 15%;
  rotate: 45deg;
  top: 10px;
  left: -23px;
  font-size: 2em;
  border: 3px solid darkgray;
  background-color: white;
  box-shadow: 2px -2px white;
}

.entry h3 {
  text-decoration: overline;
  text-decoration-color: white;
  text-decoration-thickness: 3px;
}

.entry blockquote {
  margin-left: 10px;
  margin-top: 10px;
  padding-left: 10px;
  border-left: 2px solid rgba(0, 0, 0, 0.9);
  width: 390px;
}

.titleName {
  font-size: 3em;
  font-family: 'tilt neon';
}
</style>
