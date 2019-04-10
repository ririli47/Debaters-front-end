<template>
  <div class="header">
    <nav class="navbar">
      <b class="navbar-brand"><nuxt-link class="logo" to="/">◆ Debaters</nuxt-link></b>
      <div class="navbar-end">
        <div class="navbar-item">
          <div class="buttons">
            <a class="button is-white">
              <strong>人</strong>
            </a>
            <a class="button is-white">
              <strong>Logout</strong>
            </a>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>

<style>
  .header {
    padding: 15px;
    background-color: #ffffff;
  }

  .logo {
    padding-left: 1.5em;
    margin: auto 0;
  }

  .header a:link,
  .header a:visited {
    color: #333333;
  }

  .navbar {
    width: 900px;
    margin: auto;
  }
</style>