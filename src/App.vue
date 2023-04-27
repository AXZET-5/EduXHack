<script setup>
  import Titlebar from './components/Titlebar.vue'
  import Header from './components/Header.vue'
  import Separator from './components/Separator.vue'
  import Signup from './components/Signup.vue'
  import IA from './components/IndivAd.vue'
  import IAR from './components/IndivAdRight.vue'
  import FAQ from './components/FAQ.vue'
  import Footer from './components/Footer.vue'
</script>

<script>
  export default {
    mounted() {
      var reveals = document.querySelectorAll(".Reveal");

      for (var i = 0; i < reveals.length; i++) {
        var windowHeight = window.innerHeight;
        var elementTop = reveals[i].getBoundingClientRect().top;
        var elementVisible = 0;
    
        if (elementTop < windowHeight - elementVisible) {
          reveals[i].classList.add("active");
        } else {
          reveals[i].classList.remove("active");
        }
      }
    }
  }
</script>

<template>

  <Titlebar></Titlebar>

  <Header id="home"></Header>
  
  <Separator></Separator>
  
  <Signup></Signup>
  
  <Separator></Separator>
  
  <IA
    id="content"
    imgsrc="/src/images/HCJO.png"
    title="Fundamentals"
    desc="We will be teaching HTML, CSS and JS to those without any prior experience in coding.
    Interested participants may also attend a workshop on Vue, a modern and sleek website development tool."></IA>
  <IAR
    imgsrc="/src/images/NodeJS.png"
    title="Backend development"
    desc="Stay tuned for a crash course on managing the backend of your applications with NodeJS, ExpressJS and Firebase."></IAR>
  <IA
    imgsrc="/src/images/Flutter.png"
    title="Mobile App Development"
    desc="All code written with the Flutter SDK can be deployed anywhere: Windows, Macs, IOS, Android etc.
    Learn how to use the Flutter SDK to develop cool mobile applications!"></IA>

  <Separator></Separator>

  <FAQ id="faq"></FAQ>

  <Separator></Separator>
  
  <Footer></Footer>
  
</template>

<style scoped>
</style>
