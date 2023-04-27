<template>
  <div class="TitleBarAligner"></div>
  <div class=Titlebar>
    <div class="BarGrid">
      <text class="TB Title">EduXHack</text>
      <img v-on:click="toggleHamburger" class="HamburgerIcon" src="/src/images/Hamburger.svg">
    </div>
  </div>

  <div class="Menu" id="hamburgerMenu">
    <br><br>
    <a class="MenuButton" href="#home">Home</a>
    <br><br>
    <a class="MenuButton" href="#signup">Register</a>
    <br><br>
    <a class="MenuButton" href="#content">Content</a>
    <br><br>
    <a class="MenuButton" href="#faq">FAQs</a>
  </div>
</template>

<style>
  .TitleBarAligner {
      height: 70px;
  }
  
  .Titlebar {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: rgb(50,50,50);
    z-index: 999;
    padding: 10px;
    padding-left: 40px;
    padding-right: 40px;
  }

  .TB {
    color: white;
    display: block;
  }

  .BarGrid {
    display: grid;
    grid-template-columns: auto min-content;
  }

  .HamburgerIcon {
    width: 40px;
    filter: invert(100%);
    margin-top: auto;
    margin-bottom: auto;
    margin-left: auto;
  }

  .HamburgerIcon:hover {
    cursor: pointer;
  }

  .Menu{
    position: fixed;
    top: -320px;
    right: 0px;
    z-index: 998;
    display: inline;

    background-color: rgb(50,50,50);

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
        var hamburgerMenu = document.getElementById("hamburgerMenu")
        hamburgerMenu.classList.toggle('active')
      }
    }
  }
</script>