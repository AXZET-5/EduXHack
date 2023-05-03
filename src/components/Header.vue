<template>
  <div class="Reveal Container">
    <div class="Titlegrid">
      <img class="Titleimage WithBorder" src="/src/images/IRSGlow.png">
      <div>
        <p class="Center BigTitle">EDUXHACK</p>
        <p class="Center Subtitle">EduXHack is a hackathon that aims to bring together students with diverse backgrounds and skill sets to brainstorm, design and develop innovative solutions to challenges in education</p>
        <p class="Center Await">COMING THIS JUNE</p>
      </div>
      <img class="Titleimage WithBorder" src="/src/images/EH.png">
    </div>
    <div class="Titlegrid2">
      <div class="Imagegrid">
        <img class="Titleimage2 WithBorder" src="/src/images/IRSGlow.png">
        <img class="Titleimage2 Cross" src="/src/images/x.svg">
        <img class="Titleimage2 WithBorder" src="/src/images/EH.png">
      </div>
      <div>
        <p class="Center Title">EDUXHACK</p>
        <p class="Center Subtitle">EduXHack is a hackathon that aims to bring together students with diverse backgrounds and skill sets to brainstorm, design and develop innovative solutions to challenges in education</p>
        <p class="Center Await">COMING THIS JUNE</p>
      </div>
    </div>
  </div>
</template>

<style>
  .Container {
    background-color: rgba(23, 45, 92, 0.65);
    border-radius: 40px;
    margin: 20px;
    padding: 20px;
    border: 5px solid #3D7DF5;
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
    color: rgba(225, 242, 250, 1);
  }

  .Await {
    font-size: 30px;
    letter-spacing: 3px;
    color: rgba(225, 242, 250, 1);
  }

  .Titleimage {
    border-radius: 10000px;
    width: 100%;
    margin-top: auto;
    margin-bottom: auto;
    animation: pulse 3s infinite;
  }

  .Titleimage2 {
    border-radius: 10000px;
    width: 80%;
    max-width: 200px;
    margin: auto;
    animation: pulse 3s infinite;
  }

  .Cross {
    filter: invert(1);
    animation: none;
  }

  .Imagegrid {
    display: grid;
    grid-template-columns: 4fr 1fr 4fr;
  }

  .WithBorder {
    border: 3px solid white;
  }
</style>