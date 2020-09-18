<template>
  <div class="header">
    <h1 class="heading">Oskar Kanstedt</h1>
    <img class="profilbild" src="img/oskar.jpg" alt="oskar" />
    <Buttons button-text="Startsida" to="/" class="menuButton"></Buttons>
    <Buttons button-text="Mitt CV" to="/mitt-cv" class="menuButton"></Buttons>
    <Buttons
      button-text="Övrigt om mig"
      to="/om-mig"
      class="menuButton"
    ></Buttons>
    <Buttons
      button-text="Kontakta mig"
      to="/kontakt"
      class="menuButton"
    ></Buttons>
    <br />
    <div>
      <Nuxt />
    </div>
  </div>
</template>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  margin-left: 2rem;
  margin-right: 2rem;
}

.profilbild {
  width: 10%;
  border-radius: 50%;
  align-self: right;
}

.heading {
  font-size: 400%;
}

.menuButton {
  padding: 0.2rem;
}
</style>
