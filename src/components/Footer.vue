<template>
  <div class="Footer Reveal">
    <div class="NormalFooter">
      <text class="Bold Affiliation">EduXHack</text>
      <p class="Bold Content">
        Brought to you by students from HCIRS (Hwa Chong Infocomm & Robotics
        Society)
      </p>

      <br />

      <p class="Content">Made using <u>Vue.JS</u></p>
      <p class="Content">Hosting by <u>Vercel</u></p>
      <p class="Content">
        All elements are self-created; no copyright claims infringed on.
      </p>
    </div>

    <br />

    <div class="ColumnFooter">
      <div style="padding-right: 20px">
        <p class="Bold ColumnHeader">Email</p>
        <a
          class="Content"
          target="_blank"
          href="https://mail.google.com/mail/u/0/?fs=1&tf=cm&source=mailto&to=comms@eduxhack.tech"
          >comms@eduxhack.tech</a
        >
        <br /><br />
      </div>
      <div>
        <p class="Bold ColumnHeader">Instagram</p>
        <a
          class="Content"
          target="_blank"
          href="https://www.instagram.com/eduxhack_2023/"
          >@eduxhack_2023</a
        >
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
  padding: 2rem 0;
  width: 100%;
  margin: 0;
}

@media only screen and (max-width: 500px) {
  .Footer{
    margin-left: 50px;
    margin-right: 50px;
  }
}

.NormalFooter {
  width: 80%;
}

.ColumnFooter {
  display: grid;
  grid-template-columns: 1fr 1fr;
  width: 80%;
}

@media only screen and (max-width: 500px) {
  .ColumnFooter {
    grid-template-columns: 1fr;
  }
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
