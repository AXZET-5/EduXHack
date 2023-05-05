<!--
<script setup>
  import IA from './IndivAd.vue'
  import IAR from './IndivAdRight.vue'
</script>
-->

<template>

	<p class="Center Title Reveal">Available Workshops</p>

  <div class="iLeft Reveal">
    <img class="AdImage" src="/src/images/HCJO.png">
    <div class="Container Reveal">
      <img class="InsideImage" src="/src/images/HCJO.png">
      <p class="Title">Fundamentals</p>
      <p class="Subtitle">We will be teaching HTML, CSS and JS to those without any prior experience in coding. Interested participants may also attend a workshop on Vue, a modern and sleek website development tool.</p>
    </div>
  </div>

  <div class="iRight Reveal">
    <div class="Container Reveal">
      <img class="InsideImage" src="/src/images/Express.png">
      <p class="Title">Backend development</p>
      <p class="Subtitle">Stay tuned for a crash course on managing the backend of your applications with NodeJS, ExpressJS and Firebase.</p>
    </div>
    <img class="AdImage" src="/src/images/Express.png">
  </div>

  <div class="iLeft Reveal">
    <img class="AdImage" src="/src/images/Vue.png">
    <div class="Container Reveal">
      <img class="InsideImage" src="/src/images/Vue.png">
      <p class="Title">Component-based</p>
      <p class="Subtitle">Harness the power of Vue.js to make coding your webpage efficient and elegant.</p>
    </div>
  </div>

  <div class="iRight Reveal">
    <div class="Container Reveal">
      <img class="InsideImage" src="/src/images/Flutter.png">
      <p class="Title">Mobile App Development</p>
      <p class="Subtitle">All code written with the Flutter SDK can be deployed anywhere: Windows, Macs, IOS, Android etc. <br>
    Learn how to use the Flutter SDK to develop cool mobile applications!</p>
    </div>
    <img class="AdImage" src="/src/images/Flutter.png">
  </div>

  <!--
  <IA
    imgsrc="/src/images/HCJO.png"
    title="Fundamentals"
    desc="We will be teaching HTML, CSS and JS to those without any prior experience in coding.
    Interested participants may also attend a workshop on Vue, a modern and sleek website development tool."></IA>
  <IAR
    imgsrc="/src/images/Express.png"
    title="Backend development"
    desc="Stay tuned for a crash course on managing the backend of your applications with NodeJS, ExpressJS and Firebase."></IAR>
  <IA
    imgsrc="/src/images/Vue.png"
    title="Component-based"
    desc="Harness the power of Vue.js to make coding your webpage efficient and elegant."></IA>
  <IAR
    imgsrc="/src/images/Flutter.png"
    title="Mobile App Development"
    desc="All code written with the Flutter SDK can be deployed anywhere: Windows, Macs, IOS, Android etc.
    Learn how to use the Flutter SDK to develop cool mobile applications!"></IAR>
  -->
</template>

<style>
  .iLeft {
    display: grid;
    grid-template-columns: 1fr 2fr;
  }

  .AdImage {
    height: 300px;
    display: block;
    margin-left: auto;
    margin-right: auto;
  }

  .InsideImage {
    margin-left: auto;
    margin-right: auto;
    width: 80%;
    display: none;
  }

  @media only screen and (max-width: 1000px) {
    .AdImage {
      display: none;
    }
    .InsideImage {
      display: block;
    }
    .iLeft {
      grid-template-columns: 1fr;
      margin-left: 10px;
      margin-right: 10px;
    }
  }

  .iRight {
    display: grid;
    grid-template-columns: 2fr 1fr;
  }

  @media only screen and (max-width: 1000px) {
    .iRight {
      grid-template-columns: 1fr;
      margin-left: 20px;
      margin-right: 20px;
    }
  }
</style>