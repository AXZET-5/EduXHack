<template>
  <div class="Reveal Container">
    <div class="Masthead">
      <div class="Banner">
        <img class="Titleimage WithBorder" style="background-color: #e0e2e6" src="/src/images/IRS.png" />
        <p class="Center BigTitle">EDU<span class="Accent">X</span>HACK</p>
        <img class="Titleimage WithBorder" src="/src/images/EH.png" />
      </div>
      <p class="Center Subtitle">
        EduXHack is a hackathon that aims to bring together students with
        diverse backgrounds and skill sets to brainstorm, design and develop
        innovative solutions to challenges in education
      </p>
      <a
        class="Center Await"
        href="https://docs.google.com/forms/d/e/1FAIpQLSeg5M6X7YvTHgz2_iWL71TtV24U01zJvY69PMHj8paSTyrC2g/viewform"
        target="_blank"
        >SIGN UP HERE!</a
      >
    </div>

    <div class="Masthead-SM">
      <div class="Banner">
        <div class="Imagegrid">
          <img class="Titleimage2 WithBorder" src="/src/images/IRSw.png" />
          <img class="Titleimage2 Cross" src="/src/images/x.svg" />
          <img class="Titleimage2 WithBorder" src="/src/images/EH.png" />
        </div>
        <div>
          <p class="Center Title">EDUXHACK</p>
          <p class="Center Subtitle">
            EduXHack is a hackathon that aims to bring together students with
            diverse backgrounds and skill sets to brainstorm, design and develop
            innovative solutions to challenges in education
          </p>
          <a
            class="Center Await"
            href="https://docs.google.com/forms/d/e/1FAIpQLSeg5M6X7YvTHgz2_iWL71TtV24U01zJvY69PMHj8paSTyrC2g/viewform"
            target="_blank"
            >SIGN UP HERE!</a
          >
          <br />
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.Masthead {
  display: none;
  margin-inline: 4rem;
  margin-bottom: 4rem;
}
.Masthead .Banner {
  margin-block: 4rem;
  margin-bottom: 4rem;
  display: grid;
  grid-template-columns: max(10vw, 4rem) 1fr max(10vw, 4rem);
  column-gap: 30px;
}

.Masthead-SM {
  display: block;
}
.Masthead-SM .Banner {
  display: grid;
  grid-template-columns: 1fr;
}

.Masthead .Subtitle, .Masthead-SM .Subtitle {
margin: auto;
margin-bottom: 4rem;
  }

@media only screen and (min-width: 900px) {
  .Masthead {
    display: block;
  }
  .Masthead-SM {
    display: none;
  }
}

.BigTitle {
  font-size: 64px;
  font-weight: 700;
  letter-spacing: 1rem;
  font-family: "Bruno Ace SC", Rubik, sans-serif;
}
.BigTitle .Accent {
  color: #3d7df5;
  font-size: 64px;
  font-weight: 700;
  letter-spacing: 1rem;
  font-family: "Bruno Ace SC", Rubik, sans-serif;
}

.Title {
  margin-top: 3rem;
  font-size: 35px;
  font-weight: 700;
  letter-spacing: 3px;
}

.Subtitle {
  font-size: 20px;
  line-height: 1.75rem;
  max-width: 85%;
  color: rgba(225, 242, 250, 1);
}

.Await {
  font-size: 64px;
  font-weight: 700;
  letter-spacing: 3px;
  color: rgba(225, 242, 250, 1);
  margin-top: 2rem;
}

.Titleimage {
  border-radius: 100%;
  width: 100%;
  aspect-ratio: 1/1;
  object-fit: scale-down;
  margin-top: auto;
  margin-bottom: auto;
  animation: pulse 3s infinite;
}

.Titleimage2 {
  border-radius: 10000px;
  width: 80%;
  max-width: 200px;
  margin: auto;
  animation: pulse 3s infinite;
}

.Cross {
  filter: invert(1);
  animation: none;
}

.Imagegrid {
  display: grid;
  grid-template-columns: 4fr 1fr 4fr;
}

.WithBorder {
  border: 3px solid white;
}
</style>
