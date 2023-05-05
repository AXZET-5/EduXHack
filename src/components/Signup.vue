<template>
  <div class="RegistrationParent">
    <a
      class="RegistrationChild BecomeBigger Reveal"
      href="https://docs.google.com/forms/d/e/1FAIpQLSeg5M6X7YvTHgz2_iWL71TtV24U01zJvY69PMHj8paSTyrC2g/viewform"
      target="_blank"
    >
      <p class="Center Title iRC1">SIGNUP</p>
      <p class="Center Await iRC1">TO LEARN</p>
    </a>
    <a
      class="RegistrationChild RC2 BecomeBigger Reveal"
      href="https://smartoinker.github.io/eduxhack/documents/sponsorship.pdf"
      target="_blank"
    >
      <p class="Center Title iRC2">SPONSOR</p>
      <p class="Center Await iRC2">TO TRANSCEND</p>
    </a>
  </div>

  <div class="Container Reveal">
    <p class="Center Title">About Us</p>
    <p class="Center Subtitle" style="margin-inline: auto;">
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
    border-radius: 40px !important;
    margin: 20px !important;
  }
}

.RegistrationChild {
  background-color: #3d7df5;
  margin: 20px;
  margin-left: 50px;
  margin-right: 25px;
  text-decoration: none;
  border-radius: 0px 40px 0px 40px;
  border: 15px double white;
  animation: pulse 3s infinite;
}

@keyframes pulse {
  0% {
    transform: scale(0.95);
    box-shadow: 0 0 0 0 rgba(255, 255, 255, 1);
  }

  70% {
    transform: scale(1);
    box-shadow: 0 0 0 20px rgba(255, 255, 255, 0);
  }

  100% {
    transform: scale(0.95);
    box-shadow: 0 0 0 0 rgba(255, 255, 255, 0);
  }
}

.RC2 {
  margin-left: 25px;
  margin-right: 50px;
  border-radius: 40px 0px 40px 0px;
}

.RegistrationChild:hover {
  background-color: white;
}

.RegistrationChild:hover .iRC1 {
  color: #020914;
}

.RC2:hover .iRC2 {
  color: #020914;
}
</style>
