<template>
  <div class="TitleBarAligner"></div>
  <div class="Titlebar">
    <div class="BarGrid">
      <text class="TB Title">EduXHack</text>
      <img
        v-on:click="toggleHamburger"
        class="HamburgerIcon"
        src="/src/images/Hamburger.svg"
      />
    </div>
  </div>

  <div class="Menu" id="hamburgerMenu">
    <br /><br />
    <a class="MenuButton" href="#top">Home</a>
    <br /><br />
    <a class="MenuButton" href="#signup">Workshops</a>
    <br /><br />
    <a class="MenuButton" href="#faq">Info & FAQs</a>
  </div>
</template>

<style>
.Titlebar .Title {
  margin-top: 0;
}
.TitleBarAligner {
  height: 85px;
}

.Titlebar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #020914aa;
  backdrop-filter: blur(10px);
  z-index: 999;
  padding: 15px;
  padding-left: 40px;
  padding-right: 40px;
  box-shadow: 0px 0px 10px 10px rgba(0, 0, 0, 0.5);
}

.TB {
  color: white;
  display: block;
  font-family: "Bruno Ace SC", Rubik, sans-serif;
}

.BarGrid {
  display: grid;
  grid-template-columns: auto 100px;
}

.HamburgerIcon {
  width: 40px;
  filter: invert(100%);
  margin-top: auto;
  margin-bottom: auto;
}

.HamburgerIcon:hover {
  cursor: pointer;
}

.Menu {
  position: fixed;
  top: -320px;
  right: 0px;
  z-index: 998;
  display: inline;

  background-color: #020914;
  border-left: 3px solid white;
  border-bottom: 3px solid white;

  padding: 30px;
  border-radius: 0px 0px 0px 20px;
}

.Menu.active {
  top: 20px;
}

.MenuButton {
  text-decoration: none;
  color: white;
  font-size: 30px;
}
</style>

<script>
export default {
  methods: {
    toggleHamburger() {
      var hamburgerMenu = document.getElementById('hamburgerMenu');
      hamburgerMenu.classList.toggle('active');
    },
  },
};
</script>
