<template>
  <div class="Container Opener Reveal">
    <div class="OpenerGrid" v-on:click=openSesame>
      <p class="Title">Frequently Asked Questions</p>
      <img class="TinyIcon" src="/src/images/Open.svg">
    </div>
    <div id="toOpen">
      <p class="Question">What is a hackathon?</p>
      <div class="LilBoxThingy">&nbsp</div>
      <p class="Answer">A hackathon is an invention marathon. Students come together to build cool software & hardware hacks over 24-48 hours. It’s <a href="https://medium.com/@tfogo/hackathons-are-for-beginners-77a9c9c0e000#.cj21niskl" target="_blank">very beginner friendly.</a></p>
      <br>
      <p class="Question">How much does it cost?</p>
      <div class="LilBoxThingy">&nbsp</div>
      <p class="Answer">Nothing. Attending a hackathon is free.</p>
      <br>
      <p class="Question">Do I need to be a student to attend?</p>
      <div class="LilBoxThingy">&nbsp</div>
      <p class="Answer">Yes. Only secondary school students from Singapore are eligible are eligible to attend.</p>
      <br>
      <p class="Question">Where is the event?</p>
      <div class="LilBoxThingy">&nbsp</div>
      <p class="Answer">The event is being hosted at TBC.</p>
      <br>
      <p class="Question">Is there a code of conduct?</p>
      <div class="LilBoxThingy">&nbsp</div>
      <p class="Answer">Yes there is. We enforce it very strongly. <a href="https://static.mlh.io/docs/mlh-code-of-conduct.pdf" target="_blank">You can find it here.</a></p>
    </div>
  </div>
</template>

<style>
  .Opener {
    padding-left: 200px;
    padding-right: 200px;
  }

  @media only screen and (max-width: 1200px) {
    .Opener {
      padding-left: 100px;
      padding-right: 100px;
    }
  }

  @media only screen and (max-width: 900px){
    .Opener {
      padding-left: 20px;
      padding-right: 20px;
    }
  }
  
  .OpenerGrid {
    display: grid;
    grid-template-columns: auto min-content;
  }

  .OpenerGrid:hover {
    cursor: pointer;
  }
  
  .TinyIcon {
    margin-top: auto;
    margin-bottom: auto;
    margin-left: auto;
    width: 50px;
  }

  #toOpen {
    display: none;
  }

  #toOpen.active {
    display: initial;
  }

  .LilBoxThingy {
    background-color: rgb(50,50,50);
    font-size: 10px;
    display: inline-block;
    width: 100px;
  }

  .Question {
    font-size: 25px;
    font-weight: 600;
  }

  .Answer {
    font-size: 20px;
  }
</style>

<script>
   export default {
     methods: {
       openSesame(){
         var toOpen = document.getElementById('toOpen')
         
         toOpen.classList.toggle('active')
       }
     }
   }
</script>