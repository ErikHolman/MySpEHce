<template>
  <div class="portfolioContent">
    <span class="titleName">Erik Holman</span>
    <div class="timeline">
      <div class="lines">
        <profilePics url="../assets/profile.jpg" />
      </div>
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

.lines {
  display: flex;
  flex-direction: column;
  border-top: 0;
  border-right: 1px;
  border-bottom: 0;
  border-left: 0;
  border-color: white;
  border-style: solid;
  width: 50vw;
  justify-content: stretch;
  align-items: stretch;
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
  content: '*';
  position: relative;
  top: 8px;
  left: -14px;
  transform: scale(2em);
}

.entry h3 {
  text-decoration: overline;
  text-decoration-color: white;
  border-left: 1px soild white;
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
