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
  <div class="iLeft Reveal">
    <img class="AdImage" v-bind:src=imgsrc>
    <div class="Container Reveal">
      <img class="InsideImage" v-bind:src=imgsrc>
      <p class="Title">{{title}}</p>
      <p class="Subtitle">{{desc}}</p>
    </div>
  </div>
</template>

<style>
  .iLeft {
    margin-left: 100px;
    margin-right: 100px;
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
    width: 50%;
    max-width: 150px;
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
</style>