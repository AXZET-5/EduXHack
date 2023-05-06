<template>
  <div class="Container Opener Reveal">
    <div class="OpenerGrid" v-on:click="openSesame">
      <p class="Subtitle" style="height: 2rem;">Frequently Asked Questions</p>
      <img class="TinyIcon" src="/src/images/Open.svg" id="toFlip" />
    </div>
    <div id="toOpen">
      <p class="Question">What is a hackathon?</p>
      <div class="LilBoxThingy">&nbsp</div>
      <p class="Answer">
        A hackathon is an invention marathon. Students come together to build
        cool software & hardware hacks over 24-48 hours. It’s
        <a
          href="https://medium.com/@tfogo/hackathons-are-for-beginners-77a9c9c0e000#.cj21niskl"
          target="_blank"
          >very beginner friendly.</a
        >
      </p>
      <br />
      <p class="Question">How much does it cost?</p>
      <div class="LilBoxThingy">&nbsp</div>
      <p class="Answer">Nothing. Attending a hackathon is free.</p>
      <br />
      <p class="Question">Do I need to be a student to attend?</p>
      <div class="LilBoxThingy">&nbsp</div>
      <p class="Answer">
        Yes. Only secondary school students from Singapore are eligible are
        eligible to attend.
      </p>
    </div>
  </div>
</template>

<style scoped>
.Container {
  margin-block: 6rem;
  border-bottom: 1.5px solid white;
}
.Subtitle {
  font-weight: 500;
  margin-block: 0.25rem;
}

@media only screen and (max-width: 1200px) {
  .Opener {
    padding-left: 100px;
    padding-right: 100px;
  }
}

@media only screen and (max-width: 900px) {
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
  width: 32px;
  filter: invert(1);
}

#toOpen {
  max-height: 0;
  overflow: hidden;
  transition: 0.8s max-height ease;
}

#toOpen.active {
  max-height: 40rem;
}

#toFlip {
  transform: rotate(0deg);
}

#toFlip.active {
  transform: rotate(180deg);
}

.LilBoxThingy {
  background-color: #3d7df5;
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
    openSesame() {
      var toOpen = document.getElementById('toOpen');
      var toFlip = document.getElementById('toFlip');

      toOpen.classList.toggle('active');
      toFlip.classList.toggle('active');
    },
  },
};
</script>
