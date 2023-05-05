<script setup>
import Titlebar from "./components/Titlebar.vue";
import Header from "./components/Header.vue";
import Separator from "./components/Separator.vue";
import Signup from "./components/Signup.vue";
import Content from "./components/Content.vue";
import Timeline from "./components/Timeline.vue";
import TimelineHorizontal from "./components/TimelineHorizontal.vue";
import FAQ from "./components/FAQ.vue";
import Footer from "./components/Footer.vue";
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
  },
};
</script>

<template>
  <Titlebar></Titlebar>

  <Header></Header>

  <Separator id="signup"></Separator>

  <Signup></Signup>

  <Separator id="content"></Separator>

  <Content></Content>

  <Separator id="faq"></Separator>

  <Timeline></Timeline>
  <TimelineHorizontal></TimelineHorizontal>

  <FAQ></FAQ>

  <Separator></Separator>

  <Footer></Footer>
</template>

<style scoped></style>
