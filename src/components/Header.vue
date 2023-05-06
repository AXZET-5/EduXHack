<template>
  <div class="Reveal Container">
    <div class="Masthead">
      <div class="MainTitle">
        <div class="Banner">
          <img class="Titleimage WithBorder" src="/src/images/EH.png" />
          <p class="Center BigTitle Titlename">
            EDU<span class="Accent">X</span>HACK
          </p>
        </div>
        <p class="Center Subtitle">
          EduXHack is a hackathon that aims to bring together students with
          diverse backgrounds and skill sets to brainstorm, design and develop
          innovative solutions to challenges in education
        </p>
      </div>

      <div class="MainTitle-SM">
        <div class="Banner">
          <img class="Titleimage2 WithBorder" src="/src/images/EH.png" />
          <div>
            <p class="Center Title Titlename">
              EDU<span class="Accent">X</span>HACK
            </p>
            <p class="Center Subtitle">
              EduXHack is a hackathon that aims to bring together students with
              diverse backgrounds and skill sets to brainstorm, design and
              develop innovative solutions to challenges in education
            </p>
          </div>
        </div>
      </div>
      <div class="RegistrationParent">
        <a
          class="RegistrationChild BecomeBigger Reveal"
          href="https://docs.google.com/forms/d/e/1FAIpQLSeg5M6X7YvTHgz2_iWL71TtV24U01zJvY69PMHj8paSTyrC2g/viewform"
          target="_blank"
        >
          <p class="Center Title iRC1">SIGNUP</p>
          <p class="Center ActnTitle iRC1">TO LEARN</p>
        </a>
        <a
          class="RegistrationChild RC2 BecomeBigger Reveal"
          href="https://smartoinker.github.io/eduxhack/documents/sponsorship.pdf"
          target="_blank"
        >
          <p class="Center Title iRC2">SPONSOR</p>
          <p class="Center ActnTitle iRC2">TO TRANSCEND</p>
        </a>
      </div>
    </div>
  </div>
  <div class="Container Reveal About">
    <p class="Center Title">About Us</p>
    <p class="Center Subtitle" style="margin-inline: auto">
      The hackathon is open to all students from secondary schools regardless of
      their prior experience in coding. We have arranged several workshops to
      equip participants with the necessary skills to develop their ideas. We
      believe that this event will create a platform for students to explore the
      intersection between education and technology. See below for our exciting
      workshops!
    </p>
  </div>
</template>

<style>
.MainTitle {
  display: none;
  flex-direction: column;
  align-content: center;
  margin-inline: 4rem;
}
.MainTitle .Banner {
  margin: 4rem;
  display: flex;
  justify-content: center;
  gap: 6rem;
}

.MainTitle-SM {
  display: block;
}
.MainTitle-SM .Banner {
  display: grid;
  grid-template-columns: 1fr;
}

.MainTitle .Subtitle,
.MainTitle-SM .Subtitle {
  margin: auto;
  margin-bottom: 4rem;
}

@media only screen and (min-width: 900px) {
  .Masthead {
    height: 80vh;
  }
  .MainTitle {
    display: flex;
  }
  .MainTitle-SM {
    display: none;
  }
}

.Titlename {
  font-family: "Bruno Ace SC", Rubik, sans-serif;
  margin-block: 6rem;
}
.BigTitle {
  font-size: 64px;
  font-weight: 700;
  letter-spacing: 1rem;
  font-family: "Bruno Ace SC", Rubik, sans-serif;
}
.BigTitle .Accent {
  font-size: 64px;
  font-weight: 700;
  color: #3d7df5;
  font-family: "Bruno Ace SC", Rubik, sans-serif;
}

.Title {
  margin-top: 2rem;
  font-size: 35px;
  font-weight: 700;
  letter-spacing: 3px;
}
.Title .Accent {
  font-size: 35px;
  font-weight: 700;
  color: #3d7df5;
  font-family: "Bruno Ace SC", Rubik, sans-serif;
}

.Subtitle {
  font-size: 20px;
  line-height: 1.75rem;
  max-width: 85%;
  color: rgba(225, 242, 250, 1);
}

.Titleimage {
  border-radius: 100%;
  width: 10rem;
  aspect-ratio: 1/1;
  object-fit: scale-down;
  margin-top: auto;
  margin-bottom: auto;
  animation: pulse 3s infinite;
}

.Titleimage2 {
  border-radius: 6rem;
  width: 12rem;
  margin: 2rem auto;
  animation: pulse 3s infinite;
}

.RegistrationParent {
  margin-bottom: 5rem;
  display: grid;
  grid-template-columns: 1fr 1fr;
}

@media only screen and (max-width: 800px) {
  .RegistrationParent {
    grid-template-columns: 1fr;
  }
  .RegistrationChild {
    border-radius: 20px !important;
    margin: 20px !important;
    text-align: center;
  }
  .RegistrationParent .Title {
    font-size: 20px !important;
  }
}

/* Registration action buttons */

.RegistrationChild {
  background-color: #3d7df5;
  margin: 20px;
  margin-left: 50px;
  margin-right: 25px;
  text-decoration: none;
  border-radius: 0px 40px 0px 40px;
  border: 10px double white;
  animation: pulse 3s infinite;
}
@keyframes pulse {
  0% {
    transform: scale(0.98);
    box-shadow: 0 0 0 0 rgba(255, 255, 255, 1);
  }

  70% {
    transform: scale(1);
    box-shadow: 0 0 0 5px rgba(255, 255, 255, 0);
  }

  100% {
    transform: scale(0.98);
    box-shadow: 0 0 0 0 rgba(255, 255, 255, 0);
  }
}

.RC2 {
  margin-left: 25px;
  margin-right: 50px;
  border-radius: 40px 0px 40px 0px;
}
.RegistrationChild {
  transition: 0.8s background-color ease, 0.8s color ease, 0.8s scale ease !important;
}
.RegistrationChild:hover {
  background-color: #a8c1f0;
}
.RegistrationChild:hover .iRC1,
.RC2:hover .iRC2 {
  color: #020914;
}
.RegistrationParent .Title {
  font-weight: 800;
  font-size: 32px;
}
.ActnTitle {
  font-size: 40px;
  font-weight: 700;
  letter-spacing: 3px;
  color: rgba(225, 242, 250, 1);
  margin-block: 1.25rem;
}

@media only screen and (max-width: 1200px) {
  .ActnTitle {
    font-size: 30px !important;
  }
}

.About {
  margin-top: 5rem;
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
