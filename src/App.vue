<template>
  <div id="app">
    <b-navbar toggleable="lg" type="dark" variant="dark">
      <h1>Boko no <strong style="color: #ff5733">Anime!!</strong></h1>
      <img
        src="https://i.redd.it/vvuxyi4qadf41.jpg"
        alt="อามิยะกำหมัดแล้วน้าาา"
        width="80px"
        height="75px"
      />
    </b-navbar>
    <router-view style="margin-top: none" />
  </div>
</template>

<style>
h1 {
  color: #008080;
  font-size: 40px;
  font-weight: 400;
  text-transform: uppercase;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
