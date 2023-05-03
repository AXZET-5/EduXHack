<script setup>
  import IA from './IndivAd.vue'
  import IAR from './IndivAdRight.vue'
</script>

<template>
  <p class="Center Title Reveal">Available Workshops</p>
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
</template>