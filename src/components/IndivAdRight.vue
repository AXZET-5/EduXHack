<script>
  export default {
    props: {
      imgsrc: String,
      title: String,
      desc: String,
    }
  }
</script>

<template>
  <div class="iRight Reveal">
    <div class="Container Reveal">
      <img class="InsideImage" v-bind:src=imgsrc>
      <p class="Title">{{title}}</p>
      <p class="Subtitle">{{desc}}</p>
    </div>
    <img class="AdImage" v-bind:src=imgsrc>
  </div>
</template>

<style>
  .iRight {
    margin-left: 100px;
    margin-right: 100px;
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