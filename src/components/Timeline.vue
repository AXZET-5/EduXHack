<template>
  <p class="Center Title Reveal">General Timeline</p>
  <div class="TimelineGrid">
    <div class="TheActualLine Reveal"></div>
    <div></div>
    <div
      class="Another one of TheActualLine dont question :D and also Reveal lol"
    ></div>
    <div></div>
    <div>
      <div class="Specialised Container Reveal">
        <br />
        <text class="Subtitle" style="color: white !important; font-size: 25px !important;">Signups&nbspopen!</text>
        <p class="Subtitle">4 May 2023</p>
        <a
          class="Subtitle"
          href="https://docs.google.com/forms/d/e/1FAIpQLSeg5M6X7YvTHgz2_iWL71TtV24U01zJvY69PMHj8paSTyrC2g/viewform"
          target="_blank"
          >Sign&nbspup&nbsphere!</a
        >
        <br /><br />
      </div>
      <div class="Specialised Container Reveal">
        <br />
        <text class="Subtitle" style="color: white !important; font-size: 25px !important;">Signups close</text>
        <p class="Subtitle">17 May 2023</p>
      </div>
      <div class="Specialised Container Reveal">
        <br />
        <text class="Subtitle" style="color: white !important; font-size: 25px !important;">Workshops</text>
        <p class="Subtitle">19 June 2023</p>
        <p class="Subtitle"></p>
      </div>
      <div class="Specialised Container Reveal">
        <br />
        <text class="Subtitle" style="color: white !important; font-size: 25px !important;">Hackathon!</text><br><br>
        <text class="Subtitle">20 June 2023</text><br>
        <text class="Subtitle">21 June 2023</text>
        <p class="Subtitle"></p>
      </div>
    </div>
  </div>
</template>

<style scoped>
@media only screen and (min-width: 1000px) {
  * {
    display: none;
  }
}

.TimelineGrid {
  display: grid;
  grid-template-columns: 3px 5px 3px 15px min-content;
  justify-content: center;
  margin-top: 20px;
  margin-bottom: 20px;
}

.TheActualLine {
  background-color: #3d7df5;
  height: 100%;
  width: 3px;
}

.TheActualLine.Another {
  background-color: white;
}

.Specialised {
  background-color: rgba(0, 0, 0, 0);
  border: none;
  padding-right: 0px !important;
  margin-right: 0px !important;
}
</style>
