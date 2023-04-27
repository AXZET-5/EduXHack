<template>
  <div class="RegistrationParent" id="signup">
    <a class="RegistrationChild BecomeBigger Reveal" href="https://docs.google.com/forms/d/e/1FAIpQLSeg5M6X7YvTHgz2_iWL71TtV24U01zJvY69PMHj8paSTyrC2g/viewform" target="_blank">
      <p class="Center Title iRC1">APPLY</p>
      <p class="Center Await iRC1">TO LEARN</p>
    </a>
    <a class="RegistrationChild RC2 BecomeBigger Reveal" href="https://smartoinker.github.io/eduxhack/documents/sponsorship.pdf" target="_blank">
      <p class="Center Title iRC2">SPONSOR</p>
      <p class="Center Await iRC2">TO TRANSCEND</p>
    </a>
  </div>

  <div class="Container Reveal">
    <p class="Center Title">About Us</p>
    <p class="Center Subtitle">The hackathon is open to all students from secondary schools regardless of their prior experience in coding. We have arranged several workshops to equip participants with the necessary skills to develop their ideas. We believe that this event will create a platform for students to explore the intersection between education and technology. See below for our exciting workshops!</p>
  </div>
</template>

<style>
  .RegistrationParent {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }

  @media only screen and (max-width: 800px){
    .RegistrationParent {
      grid-template-columns: 1fr;
    }
  }

  .RegistrationChild {
    background-color: #d1fffd;
    margin: 20px;
    text-decoration: none;
    border-radius: 20px;
    border: 5px solid #c2e4ff;
  }

  .RC2 {
    background-color: #fff7d1;
    border: 5px solid #ffeea8;
  }

  .RegistrationChild:hover {
    background-color: rgb(50,50,50);
  }

  .RegistrationChild:hover .iRC1 {
    color: #d1fffd;
  }
  
  .RC2:hover .iRC2 {
    color: #fff7d1;
  }
</style>