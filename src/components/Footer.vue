<template>
  <div class="Footer Reveal">

    <div class="NormalFooter">
      <text class="Bold Affiliation">EduXHack</text>
      <p class="Bold Content">Brought to you by HCIRS (Hwa Chong Infocomm & Robotics Society)</p>
  
      <br>
      
      <p class="Content">Made using <u>Vue.JS</u></p>
      <p class="Content">Hosting by <u>Vercel</u></p>
      <p class="Content">All elements are self-created; no copyright claims infringed on.</p>
    </div>

    <br>
    
    <div class="ColumnFooter">
      <div style="padding-right: 20px">
      <p class="Bold ColumnHeader">Email</p>
      <a class="Content" target="_blank" href="https://mail.google.com/mail/u/0/?fs=1&tf=cm&source=mailto&to=eduxhackhttpsociety@gmail.com">admin@eduxhack.tech</a>
      </div>
      <div>
      <p class="Bold ColumnHeader">Instagram</p>
      <a class="Content" target="_blank" href="https://www.instagram.com/eduxhack_2023/">@eduxhack_2023</a>
      </div>
    </div>
  </div>
</template>

<style scoped>
  u {
    color: white;
  }
  .Logo {
    width: 50px;
    display: inline;
    filter: saturate(4);
    filter: brightness(1.5);
  }
  .Inline {
    display: inline;
  }
  
  .Footer {
    padding-top: 35px;
    padding-bottom: 35px;
    width: 100%;
    margin: 0;
  }

  .NormalFooter {
    width: 80%;
    margin-left: auto;
    margin-right: auto;
  }

  .ColumnFooter {
    display: grid;
    grid-template-columns: 1fr 1fr;
    width: 80%;
    margin-left: auto;
    margin-right: auto;
  }

  .Affiliation {
    color: white;
    font-family: Segoe UI, -apple-system, sans-serif;
    font-size: 30px;
    vertical-align: top;
  }

  .ColumnHeader {
    color: white;
    font-family: Segoe UI, -apple-system, sans-serif;
    font-size: 20px;
  }
  
  .Content {
    color: white;
    font-family: Segoe UI, -apple-system, sans-serif;
    padding-bottom: 5px;
  }

  .Center {
    text-align: center;
  }

  .Bold {
    font-weight: 600;
  }
</style>