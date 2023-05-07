<template>
  <div class="Whole">
    <div class="TimelineGrid">
      <div class="Specialised Reveal">
        <br />
        <text class="Timelined Title">Signups&nbspopen!</text><br><br>
        <text class="Center Subtitle">4 May 2023</text><br><br>
        <text class="Subtitle">/\</text>
      </div>
      <div class="Specialised Reveal">
        <br />
        <text class="Timelined Title">Signups close</text><br><br>
        <text class="Center Subtitle">17 May 2023</text><br><br>
        <text class="Subtitle">/\</text>
      </div>
      <div class="Specialised Reveal">
        <br />
        <text class="Timelined Title">Workshops</text><br><br>
        <text class="Center Subtitle">19 June 2023</text><br><br>
        <text class="Subtitle">/\</text>
      </div>
      <div class="Specialised Reveal">
        <br />
        <text class="Timelined Title">Hackathon!</text><br><br>
        <text class="Center Subtitle">20-21 June 2023</text><br><br>
        <text class="Subtitle">/\</text>
      </div>
    </div>
    <div class="HorizontalLine Reveal"></div>
    <div style="height: 5px"></div>
    <div class="Another HorizontalLine Reveal"></div>
  </div>
  <br /><br />
</template>

<style scoped>
@media only screen and (max-width: 1000px) {
  * {
    display: none;
  }
}

.TimelineGrid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
}

.HorizontalLine {
  background-color: white;
  width: 100%;
  height: 2px;
  margin-inline: -50px !important;
  padding-inline: 50px !important;
}

.HorizontalLine.Another {
  background-color: #3d7df5;
}

.Specialised {
  text-align: center;
  width: 100% !important;
  background-color: rgba(0, 0, 0, 0);
  border: none;
  margin-inline: 10px;
  margin-bottom: -25px;
}

.Timelined {
  font-size: 24px;
  letter-spacing: 0px;
}

@media only screen and (max-width: 1250px) {
  .Timelined {
    font-size: 25px;
  }
}

.Whole {
  margin-left: 50px;
  margin-right: 50px;
}
</style>
