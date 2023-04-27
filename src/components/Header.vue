<template>
  <div class="Reveal Container">
    <div class="Titlegrid">
      <img class="Titleimage WithBorder BecomeBigger" src="/src/images/IRS.png">
      <div>
        <p class="Center BigTitle BecomeBigger">EDUXHACK</p>
        <p class="Center Subtitle BecomeBigger">EduXHack is a hackathon that aims to bring together students with diverse backgrounds and skill sets to brainstorm, design and develop innovative solutions to challenges in education</p>
        <p class="Center Await BecomeBigger">COMING THIS JUNE</p>
      </div>
      <img class="Titleimage BecomeBigger" src="/src/images/EH.jpg">
    </div>
    <div class="Titlegrid2">
      <div class="Imagegrid">
        <img class="Titleimage2 WithBorder BecomeBigger" src="/src/images/IRS.png">
        <img class="Titleimage2 BecomeBigger" src="/src/images/x.svg">
        <img class="Titleimage2 BecomeBigger" src="/src/images/EH.jpg">
      </div>
      <div>
        <p class="Center Title BecomeBigger">EDUXHACK</p>
        <p class="Center Subtitle BecomeBigger">EduXHack is a hackathon that aims to bring together students with diverse backgrounds and skill sets to brainstorm, design and develop innovative solutions to challenges in education</p>
        <p class="Center Await BecomeBigger">COMING THIS JUNE</p>
      </div>
    </div>
  </div>
</template>

<style>
  .Container {
    background-color: rgb(235,235,235);
    border-radius: 40px;
    margin: 20px;
    padding: 20px;
  }

  .Titlegrid {
    display: grid;
    grid-template-columns: 1fr 3fr 1fr;
    column-gap: 30px;
  }
  
  .Titlegrid2 {
    display: none;
    grid-template-columns: 1fr;
  }

  @media only screen and (max-width: 800px){
    .Titlegrid{
      display: none;
    }
    .Titlegrid2{
      display: grid;
    }
  }
  
  .BigTitle {
    font-size: 40px;
    font-weight: 700;
    letter-spacing: 3px;
  }

  .Title {
    font-size: 35px;
    font-weight: 700;
    letter-spacing: 3px;
  }

  .Subtitle {
    font-size: 20px;
    font-weight: 600;
    color: rgb(120,120,120);
  }

  .Await {
    font-size: 30px;
    letter-spacing: 3px;
    color: rgb(120,120,120);
  }

  .Titleimage {
    border-radius: 10000px;
    width: 100%;
    margin-top: auto;
    margin-bottom: auto;
  }

  .Titleimage2 {
    border-radius: 10000px;
    width: 80%;
    max-width: 200px;
    margin: auto;
  }

  .Imagegrid {
    display: grid;
    grid-template-columns: 4fr 1fr 4fr;
  }

  .WithBorder {
    border: 5px solid rgb(100,100,100);
  }
</style>