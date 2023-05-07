<template>
  <p class="Center Title Reveal">Available Workshops</p>

  <div class="Workshops">
    <div class="iLeft Reveal">
      <img class="AdImage" src="/src/images/HCJO.svg" />
      <div class="Container Reveal">
        <img class="InsideImage" src="/src/images/HCJO.svg" />
        <p class="Whatever Title">Fundamentals</p>
        <p class="Whatever Subtitle">
          We will be teaching HTML, CSS and JS to those without any prior
          experience in coding. Interested participants may also attend a
          workshop on Vue, a modern and sleek website development tool.
        </p>
      </div>
    </div>

    <div class="iRight Reveal">
      <div class="Container Reveal">
        <img class="InsideImage" src="/src/images/Express.svg" />
        <p class="Whatever Title">Backend Development</p>
        <p class="Whatever Subtitle">
          Stay tuned for a crash course on managing the backend of your
          applications with NodeJS, ExpressJS and Firebase.
        </p>
      </div>
      <img class="AdImage" src="/src/images/Express.svg" />
    </div>

    <div class="iLeft Reveal">
      <img class="AdImage" src="/src/images/Vue.svg" />
      <div class="Container Reveal">
        <img class="InsideImage" src="/src/images/Vue.svg" />
        <p class="Whatever Title">Component Framework</p>
        <p class="Whatever Subtitle">
          Harness the power of Vue.js to make coding your webpage efficient and
          elegant.
        </p>
      </div>
    </div>

    <div class="iRight Reveal">
      <div class="Container Reveal">
        <img class="InsideImage" src="/src/images/Flutter.svg" />
        <p class="Whatever Title">Mobile App Development</p>
        <p class="Whatever Subtitle">
          All code written with the Flutter SDK can be deployed anywhere:
          Windows, Macs, IOS, Android etc. <br />
          Learn how to use the Flutter SDK to develop cool mobile applications!
        </p>
      </div>
      <img class="AdImage" src="/src/images/Flutter.svg" />
    </div>
  </div>
</template>

<style>
.Workshops {
  margin-bottom: 8rem;
}
.iLeft,
.iRight {
  display: grid;
  grid-gap: 2rem;
  align-items: center;
}
.iLeft {
  grid-template-columns: 1fr 4fr;
}
.iRight {
  grid-template-columns: 4fr 1fr;
}

.AdImage {
  height: 250px;
  display: block;
  margin-left: auto;
  margin-right: auto;
}

.InsideImage {
  margin-left: auto;
  margin-right: auto;
  width: min(80%, 12rem);
  display: none;
}

@media only screen and (max-width: 1000px) {
  .AdImage {
    display: none;
  }

  @media only screen and (min-width: 600px) {
    .InsideImage {
      width: 60%;
    }
  }

  @media only screen and (min-width: 700px) {
    .InsideImage {
      width: 40%;
    }
  }

  @media only screen and (min-width: 800px) {
    .InsideImage {
      width: 30%;
    }
  }

  .FlutterInsideImage {
    margin-left: auto;
    margin-right: auto;
    width: 150px;
    display: none;
  }

  @media only screen and (max-width: 1000px) {
    .AdImage {
      display: none;
    }
    .InsideImage {
      display: block;
    }
    .FlutterInsideImage {
      display: block;
    }
    .iLeft {
      grid-template-columns: 1fr;
      margin-left: 10px;
      margin-right: 10px;
    }
    .iRight {
      grid-template-columns: 1fr !important;
      margin-left: 10px;
      margin-right: 10px;
    }
    .Whatever {
      text-align: center;
      margin-left: auto !important;
      margin-right: auto !important;
    }
  }
  .iLeft {
    grid-template-columns: 1fr;
    margin-left: 10px;
    margin-right: 10px;
  }
  .iLeft,
  .iRight {
    margin-top: trem;
  }
}

@media only screen and (max-width: 1000px) {
  .iRight {
    display: grid;
    grid-template-columns: 2fr 1fr;
  }
}
</style>
